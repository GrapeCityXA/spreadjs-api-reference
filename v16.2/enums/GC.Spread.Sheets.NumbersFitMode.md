# Enumeration: NumbersFitMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).NumbersFitMode

当日期/数字数据宽度大于列宽度时,改变显示模式

**`代码示例`**
```
//本例使用NumbersFitMode枚举
spread.options.numbersFitMode = GC.Spread.Sheets.NumbersFitMode.overflow;
```

## Table of contents

### Enumeration members

- [mask](GC.Spread.Sheets.NumbersFitMode.md#mask)
- [overflow](GC.Spread.Sheets.NumbersFitMode.md#overflow)

## Enumeration members

### <a id="mask" name="mask"></a> mask

• **mask** = `0`

Indicates replacing data content with "###" and show tip.

___

### <a id="overflow" name="overflow"></a> overflow

• **overflow** = `1`

以字符串形式显示数据内容,如果下一个单元格为空,则溢出该内容
