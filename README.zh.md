# SpreadJS API 文档

SpreadJS 完整 API 参考，纯文本 Markdown，按版本分目录。这份说明主要给 AI 编码助手读：定位和解析符号需要的信息都在下面。

[English](README.md) | **中文**

---

## 这是什么

每个 `v<版本>/` 目录是一份完整的 API 参考，由 TypeDoc 从 SpreadJS 源码注释生成。说明文字是中文，签名、类型名和示例代码与语言无关。

## 定位一个符号

**不要用类名拼路径。** 文件名通常等于完整限定名，但两个实体重名时 TypeDoc 会追加 `-1`（全库有 23 个这样的文件，比如 `v19.1/excelio/classes/GC.Spread.Excel.IO-1.md`）。先搜再读：

```bash
# 找定义某个类的文件
find . -name "GC.Spread.Sheets.Worksheet.md" -not -path "./.git/*"

# 只知道短名时，按标题搜
grep -rln "^# Class: Worksheet$" v19.1/

# 找提到某个成员的所有位置
grep -rn "getActiveSheet" v19.1/classes/GC.Spread.Sheets.Workbook.md
```

## 各类内容的位置

| 符号类型 | `v19.1/` 下的路径 |
| --- | --- |
| 命名空间 / 模块 | `modules/GC.Spread.Sheets.md` —— **入口，从这里开始** |
| 类 | `classes/GC.Spread.Sheets.Worksheet.md` |
| 接口 | `interfaces/GC.Spread.Sheets.ISize.md` |
| 枚举 | `enums/GC.Spread.Sheets.HorizontalAlign.md` |
| 设计器组件 | `designer/{modules,classes,interfaces,enums}/` |
| Excel 导入导出 | `excelio/{modules,classes,enums}/` —— **没有 `interfaces/`** |
| 协同组件 | `collaboration/<npm 包名>/{classes,enums,interfaces}/` + `Overview.md` |

`modules/` 是索引层。每个文件描述一个命名空间，链出它的类、接口、枚举和函数。先读它能低成本拿到整体认识，再决定打开哪个类型文件。

`designer`、`excelio`、`collaboration` 三棵树各自独立，都有自己的 `modules/`，**不会**出现在根目录的 `modules/` 里。有两点需要留意：

- `collaboration/` 多一层包名（共 10 个包：`js-collaboration`、`js-collaboration-ot`、`spread-sheets-collaboration` 等）。每个包有自己的 `Overview.md`，其中 `js-collaboration-presence/` 只有 `Overview.md`。这里的文件名不带 `GC.Spread.*` 前缀，是裸名，如 `interfaces/IChangeSet.md`。
- `designer/` 的文件名保留完整的 `GC.Spread.Sheets.Designer.*` 前缀。

## 文件结构

每个文件的结构一致，标记含义如下：

```markdown
# Class: Worksheet                    ← 类型 + 短名。类型 ∈ Class | Interface |
                                        Enumeration | Namespace
[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Worksheet
                                       ← 面包屑 = 父级链，链接都是相对路径
## Hierarchy                           ← 仅类有；↳ 标记子类
## Table of contents                   ← 成员索引，跳转到锚点
### <a id="getrange" name="getrange"></a> getRange
                                       ← 锚点 id 是成员名的小写形式
▸ **getRange**(`row`, `col`, `rowCount?`, ...): [`CellRange`](GC.Spread.Sheets.CellRange.md)
#### Parameters
| Name | Type | Description |       ← 参数名带 `?` 后缀表示可选
#### Returns
```

成员标记：

| 标记 | 含义 |
| --- | --- |
| `▸` | 方法（或函数） |
| `•` | 属性、枚举成员或变量 |
| `• **new X**()` | 构造函数 |
| `` • `Static` **X**: `string` `` | 静态成员 |
| `` • **x** = `1` `` | 枚举成员及其数值 |
| `___` | 成员之间的分隔线 |
| `` **`example`** `` + ` ```javascript ` | 可直接运行的示例，最可靠的用法来源 |
| `` **`param`** `` | 描述事件参数的字段 |

两处容易解析错的地方：

- **重载共用同一个标题。** 一个方法有多个签名时，多个 `▸ **名字**(...)` 块会堆在同一个锚点下。下结论前要把它们都读完。`Worksheet.getRange` 就有两个。
- **事件是普通字符串常量**，不是带类型的 emitter：`` • `Static` **CurrentUserChanged**: `string` ``。事件定义在 `Events` 类里（`GC.Spread.Sheets.Events`、`GC.Spread.Sheets.Designer.Events`、`GC.Spread.Common.Events`）。

**链接到具体成员**：`<文件名>.md#<成员名小写>`，例如 `classes/GC.Spread.Sheets.Worksheet.md#getrange`。重载共用同一个锚点。

## 中文说明怎么看

类型名、签名和代码示例不用翻译，直接读。只有散文部分是中文，而且措辞高度模式化，按位置就能解析：

| 中文 | 含义 |
| --- | --- |
| 表示… | 定义 |
| 如果未提供此参数，则默认值为 X | 省略该参数时的默认值 |
| 获取… / 设置… | getter / setter |
| 此示例… | 引出示例代码 |

`Description` 列和 `#### Returns` 之后的文字是权威的行为说明，里面常有签名表达不了的约束。

## toc.json

每个版本带一份 `toc.json`（约 924 KB，1263 条），是原文档站的导航树。有用的字段：`Text`（完整限定名）、`DisplayName`、`Type`（`Api` | `ApiAppend` | `file`）、`DocumentPath`、`ParentId`。

`Type` 为 `"Api"` 的条目，文件路径是 `<版本>` + `DocumentPath` + `.md`。

**它适合看结构，不适合做精确定位。** `Text` 和 `DisplayName` 都不是唯一键（分别有 30 和 43 个重名），`Type` 为 `"file"` 的条目是导航分组，没有对应文件。`v18.0` 干脆没有 `toc.json`。要定位具体符号就 `grep` Markdown，那个永远准。

## 版本

| 版本 | 说明 |
| --- | --- |
| v16.2 | |
| v17.0 | |
| v17.1 | |
| v18.0 | 新增 collaboration；无 `toc.json` |
| v18.1 | |
| v18.2 | |
| v19.0 | |
| v19.1 | 当前最新 |

想确认某个 API 什么时候出现的，跨版本搜，缺哪个版本就是当时还没有：

```bash
grep -rln "DataCharts" v16.2/ v17.0/ v17.1/ v18.0/ v18.1/ v18.2/ v19.0/ v19.1/
# → v18.0 起才有（DataCharts 是 v18.0 引入的）
```

## 其他注意点

- `excelio/` 没有 `interfaces/` 目录，它的 `classes/` 只有一个文件。
- `collaboration/` 在 v18.0 之前不存在。
- `-1` 后缀表示重名冲突，与版本和重载无关。
- 根 `modules/` 只覆盖核心库。设计器、ExcelIO 和协同的 API **不在**里面，要去各自的树。
- 说明文字可能滞后或比代码简略。关键行为请对照[官方文档](https://www.grapecity.com.cn/developer/spreadjs)核实。

## 说明

SpreadJS 是西安葡萄城（GrapeCity）的商用 JavaScript 表格控件。本仓库内容由官方 API 文档生成，仅供查阅参考；SpreadJS 及相关名称、标识的权利归葡萄城所有。实际开发请以[官网](https://www.grapecity.com.cn/developer/spreadjs)发布的信息和随附的产品许可协议为准。
