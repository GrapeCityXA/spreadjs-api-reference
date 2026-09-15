# Enumeration: InvalidOperationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).InvalidOperationType

标识哪个操作无效。

**`example`**
```javascript
//此示例获取无效类型。
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
- [sizeLimitExceeded](GC.Spread.Sheets.InvalidOperationType.md#sizelimitexceeded)
- [sort](GC.Spread.Sheets.InvalidOperationType.md#sort)
- [table](GC.Spread.Sheets.InvalidOperationType.md#table)

## Enumeration members

### <a id="changepartofarrayformula" name="changepartofarrayformula"></a> changePartOfArrayFormula

• **changePartOfArrayFormula** = `4`

指定插入行无效。

___

### <a id="changesheetname" name="changesheetname"></a> changeSheetName

• **changeSheetName** = `5`

指定更改的工作表名称无效。

___

### <a id="copypaste" name="copypaste"></a> copyPaste

• **copyPaste** = `1`

指定复制粘贴无效。

___

### <a id="customname" name="customname"></a> customName

• **customName** = `15`

指定要设置为自定义名称的值有效。

___

### <a id="cutprotected" name="cutprotected"></a> cutProtected

• **cutProtected** = `14`

指定单元格被锁定且工作表受保护时剪切值无效。

___

### <a id="dataobjectcelltypeinsertdata" name="dataobjectcelltypeinsertdata"></a> dataObjectCellTypeInsertData

• **dataObjectCellTypeInsertData** = `16`

指定数据对象单元格类型不能在其右侧相邻单元格中插入数据。

___

### <a id="dragdrop" name="dragdrop"></a> dragDrop

• **dragDrop** = `3`

指定拖拽放置无效。

___

### <a id="dragfill" name="dragfill"></a> dragFill

• **dragFill** = `2`

指定拖拽填充无效。

___

### <a id="editprotected" name="editprotected"></a> editProtected

• **editProtected** = `13`

指定单元格被锁定且工作表受保护时编辑值无效。

___

### <a id="filter" name="filter"></a> filter

• **filter** = `7`

指定添加筛选无效。

___

### <a id="groupprotected" name="groupprotected"></a> groupProtected

• **groupProtected** = `12`

指定工作表未保护时组可以展开和折叠。

___

### <a id="pivottable" name="pivottable"></a> pivotTable

• **pivotTable** = `10`

指定更改影响已存在的数据透视表。

___

### <a id="ptoverlapvalue" name="ptoverlapvalue"></a> ptOverlapValue

• **ptOverlapValue** = `11`

指定数据透视表更改将覆盖有值的单元格。

___

### <a id="setformula" name="setformula"></a> setFormula

• **setFormula** = `0`

指定公式无效。

___

### <a id="sizelimitexceeded" name="sizelimitexceeded"></a> sizeLimitExceeded

• **sizeLimitExceeded** = `18`

当通过文件选择器上传的文件大小超过限制时触发的特定事件类型。

___

### <a id="sort" name="sort"></a> sort

• **sort** = `9`

指定排序无效。

___

### <a id="table" name="table"></a> table

• **table** = `6`

指定表格操作无效。
