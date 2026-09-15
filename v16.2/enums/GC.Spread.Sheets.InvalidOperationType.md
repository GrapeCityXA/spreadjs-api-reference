# Enumeration: InvalidOperationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).InvalidOperationType

标识操作为无效

**`代码示例`**
```
//本示例获取无效的类型
activeSheet.getCell(1,1).locked(true);
activeSheet.options.isProtected = true;
activeSheet.getCell(1,1).value(2);
//绑定事件
activeSheet.bind(GC.Spread.Sheets.Events.InvalidOperation, function (e, info) {
        alert("Message (" + info.invalidType + ")");
});
```

## Table of contents

### Enumeration members

- [changePartOfArrayFormula](GC.Spread.Sheets.InvalidOperationType.md#changepartofarrayformula)
- [changeSheetName](GC.Spread.Sheets.InvalidOperationType.md#changesheetname)
- [copyPaste](GC.Spread.Sheets.InvalidOperationType.md#copypaste)
- [customName](GC.Spread.Sheets.InvalidOperationType.md#customname)
- [cutProtected](GC.Spread.Sheets.InvalidOperationType.md#cutprotected)
- [dataObjectCellTypeInsertData](GC.Spread.Sheets.InvalidOperationType.md#dataobjectcelltypeinsertdata)
- [dragDrop](GC.Spread.Sheets.InvalidOperationType.md#dragdrop)
- [dragFill](GC.Spread.Sheets.InvalidOperationType.md#dragfill)
- [editProtected](GC.Spread.Sheets.InvalidOperationType.md#editprotected)
- [filter](GC.Spread.Sheets.InvalidOperationType.md#filter)
- [groupProtected](GC.Spread.Sheets.InvalidOperationType.md#groupprotected)
- [pivotTable](GC.Spread.Sheets.InvalidOperationType.md#pivottable)
- [ptOverlapValue](GC.Spread.Sheets.InvalidOperationType.md#ptoverlapvalue)
- [setFormula](GC.Spread.Sheets.InvalidOperationType.md#setformula)
- [sort](GC.Spread.Sheets.InvalidOperationType.md#sort)
- [table](GC.Spread.Sheets.InvalidOperationType.md#table)

## Enumeration members

### <a id="changepartofarrayformula" name="changepartofarrayformula"></a> changePartOfArrayFormula

• **changePartOfArrayFormula** = `4`

插入行无效

___

### <a id="changesheetname" name="changesheetname"></a> changeSheetName

• **changeSheetName** = `5`

更改的表单名称无效

___

### <a id="copypaste" name="copypaste"></a> copyPaste

• **copyPaste** = `1`

复制粘贴无效

___

### <a id="customname" name="customname"></a> customName

• **customName** = `15`

指定要设置为自定义名称的值有效。

___

### <a id="cutprotected" name="cutprotected"></a> cutProtected

• **cutProtected** = `14`

单元格锁定且工作表受保护时的剪切值。

___

### <a id="dataobjectcelltypeinsertdata" name="dataobjectcelltypeinsertdata"></a> dataObjectCellTypeInsertData

• **dataObjectCellTypeInsertData** = `16`

数据对象单元格类型无法将数据插入到其右侧的相邻单元格中。

___

### <a id="dragdrop" name="dragdrop"></a> dragDrop

• **dragDrop** = `3`

拖放无效

___

### <a id="dragfill" name="dragfill"></a> dragFill

• **dragFill** = `2`

拖动填充无效

___

### <a id="editprotected" name="editprotected"></a> editProtected

• **editProtected** = `13`

单元格锁定且工作表受保护时的编辑值

___

### <a id="filter" name="filter"></a> filter

• **filter** = `7`

添加的筛选无效

___

### <a id="groupprotected" name="groupprotected"></a> groupProtected

• **groupProtected** = `12`

工作表未受保护时可以展开和折叠的组

___

### <a id="pivottable" name="pivottable"></a> pivotTable

• **pivotTable** = `10`

更改影响已存在的透视表

___

### <a id="ptoverlapvalue" name="ptoverlapvalue"></a> ptOverlapValue

• **ptOverlapValue** = `11`

数据透视表更改将重叠有值的单元格

___

### <a id="setformula" name="setformula"></a> setFormula

• **setFormula** = `0`

公式无效

___

### <a id="sort" name="sort"></a> sort

• **sort** = `9`

排序无效。

___

### <a id="table" name="table"></a> table

• **table** = `6`

添加的表格行为无效
