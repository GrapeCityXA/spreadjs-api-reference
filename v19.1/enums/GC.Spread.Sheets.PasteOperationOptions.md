# Enumeration: PasteOperationOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).PasteOperationOptions

指定复制和粘贴范围之间数学组合值的操作选项

**`example`**
```javascript
//此示例使用PasteOperationOptions枚举。
activeSheet.getCell(0,0).value("1");
activeSheet.setSelection(0, 0, 1, 1);
spread.commandManager().execute({cmd:"copy", sheetName: activeSheet.name()});
activeSheet.setSelection(0, 0, 3, 3);
spread.commandManager().execute(
    {
        cmd:"paste",
        sheetName: activeSheet.name(),
        pasteSpecialOptions: {
            operationOptions: GC.Spread.Sheets.PasteOperationOptions.add
        }
    }
);
```

## Table of contents

### Enumeration members

- [add](GC.Spread.Sheets.PasteOperationOptions.md#add)
- [divide](GC.Spread.Sheets.PasteOperationOptions.md#divide)
- [multiply](GC.Spread.Sheets.PasteOperationOptions.md#multiply)
- [none](GC.Spread.Sheets.PasteOperationOptions.md#none)
- [subtract](GC.Spread.Sheets.PasteOperationOptions.md#subtract)
- [transform](GC.Spread.Sheets.PasteOperationOptions.md#transform)

## Enumeration members

### <a id="add" name="add"></a> add

• **add** = `1`

将复制范围的值添加到粘贴范围的值中。

___

### <a id="divide" name="divide"></a> divide

• **divide** = `4`

将粘贴范围的值除以复制范围的值。

___

### <a id="multiply" name="multiply"></a> multiply

• **multiply** = `3`

将粘贴范围的值乘以复制范围的值。

___

### <a id="none" name="none"></a> none

• **none** = `0`

不进行任何操作直接粘贴复制范围的内容。

___

### <a id="subtract" name="subtract"></a> subtract

• **subtract** = `2`

从粘贴范围的值中减去复制范围的值。

___

### <a id="transform" name="transform"></a> transform

• **transform** = `5`

通过复制区域中的公式转换粘贴区域中的值。
