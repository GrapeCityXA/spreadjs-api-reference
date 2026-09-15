# Enumeration: PasteOperationOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).PasteOperationOptions

指定操作选项，在复制范围和粘贴范围之间以数学方式进行值的合并

**`example`**
```
//This example uses the PasteOperationOptions enumeration.
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

## Enumeration members

### <a id="add" name="add"></a> add

• **add** = `1`

将复制范围中的值加上粘贴范围中的值

___

### <a id="divide" name="divide"></a> divide

• **divide** = `4`

将粘贴范围中的值除以复制范围中的值

___

### <a id="multiply" name="multiply"></a> multiply

• **multiply** = `3`

将粘贴范围中的值乘以复制范围中的值

___

### <a id="none" name="none"></a> none

• **none** = `0`

将复制范围的内容粘贴到目标区域，不执行任何操作

___

### <a id="subtract" name="subtract"></a> subtract

• **subtract** = `2`

将粘贴范围中的值减去复制范围中的值
