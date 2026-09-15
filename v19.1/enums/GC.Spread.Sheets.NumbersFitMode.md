# Enumeration: NumbersFitMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).NumbersFitMode

当日期/数字数据宽度超过列宽时的显示模式。

**`example`**
```javascript
//此示例使用NumbersFitMode枚举。
spread.options.numbersFitMode = GC.Spread.Sheets.NumbersFitMode.overflow;
```

## Table of contents

### Enumeration members

- [mask](GC.Spread.Sheets.NumbersFitMode.md#mask)
- [overflow](GC.Spread.Sheets.NumbersFitMode.md#overflow)

## Enumeration members

### <a id="mask" name="mask"></a> mask

• **mask** = `0`

表示用"###"替换数据内容并显示提示。

___

### <a id="overflow" name="overflow"></a> overflow

• **overflow** = `1`

表示以字符串形式显示数据内容，如果下一个单元格为空，则内容会溢出显示。
