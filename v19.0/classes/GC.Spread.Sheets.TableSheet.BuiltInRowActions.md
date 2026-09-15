# Class: BuiltInRowActions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).BuiltInRowActions

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#constructor)

### Properties

- [dirtyStatus](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#dirtystatus)
- [pinRow](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#pinrow)
- [removeRow](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#removerow)
- [resetRow](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#resetrow)
- [saveRow](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#saverow)
- [warningInfo](GC.Spread.Sheets.TableSheet.BuiltInRowActions.md#warninginfo)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new BuiltInRowActions**()

表示计算表的内置行操作。

## Properties

### <a id="dirtystatus" name="dirtystatus"></a> dirtyStatus

▪ `Static` **dirtyStatus**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示行中的数据更改

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} dirtyStatus - 显示行中的数据更改。

**`example`**
```javascript
// 当数据发生更改时，“脏数据”状态将显示在表格工作表中相应的行上。
var dataManager = spread.dataManager();
var myTable = dataManager.addTable("myTable", {
    autoSync:true,
    remote: {
        read: {
            url: 'https://demodata.grapecity.com/northwind/api/v1/Orders'
        }
    }
});
myTable.fetch().then(function() {
    var myView = myTable.addView("myView");
    var tableSheet = spread.addSheetTab(1, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
    tableSheet.setDataView(myView);
    let sheet = spread.sheets[0];
    sheet.setRowCount(myTable.length() + 1);
    sheet.setColumnCount(Object.keys(myTable.columns).length + 1);
    sheet.tables.addFromDataSource("Table1", 0, 0, "myTable", GC.Spread.Sheets.Tables.TableThemes.dark1);
    sheet.setValue(1, 0, 'new value');
});
```

___

### <a id="pinrow" name="pinrow"></a> pinRow

▪ `Static` **pinRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示固定行。

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} pinRow - 固定行。

**`example`**
```javascript
// 当某些行被固定时，会显示固定状态
tableSheet.togglePinnedRows([1,2,4]);
```

___

### <a id="removerow" name="removerow"></a> removeRow

▪ `Static` **removeRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示删除行。

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} removeRow - 删除行。

**`example`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="resetrow" name="resetrow"></a> resetRow

▪ `Static` **resetRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示重置数据更改。

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} resetRow - 重置行中的数据更改。

**`example`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="saverow" name="saverow"></a> saveRow

▪ `Static` **saveRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示保存行中的数据更改。

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} saveRow - 保存行中的数据更改。

**`example`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="warninginfo" name="warninginfo"></a> warningInfo

▪ `Static` **warningInfo**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

表示警告信息的文本。

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} warningInfo - 在行中显示警告信息。

**`example`**
```javascript
// 当远程请求失败时，警告状态将显示在表格工作表中相应的行上。
var dataManager = spread.dataManager();
var myTable = dataManager.addTable("myTable", {
    autoSync:true,
    remote: {
        read: {
            url: 'https://demodata.grapecity.com/northwind/api/v1/Orders'
        },
        create: {
            url: 'https://invalidurl'
        }
    }
});
myTable.fetch().then(function() {
    var myView = myTable.addView("myView");
    var tableSheet = spread.addSheetTab(1, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
    tableSheet.setDataView(myView);
    tableSheet.addRow({id: 8, name: "spreadjs"});
});
```
