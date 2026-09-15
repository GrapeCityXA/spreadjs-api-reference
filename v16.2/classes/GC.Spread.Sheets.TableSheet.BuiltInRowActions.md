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

Represent the table sheet built-in row actions.

## Properties

### <a id="dirtystatus" name="dirtystatus"></a> dirtyStatus

▪ `Static` **dirtyStatus**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} dirtyStatus - 显示行数据变化

___

### <a id="pinrow" name="pinrow"></a> pinRow

▪ `Static` **pinRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} pinRow - 钉上一行

___

### <a id="removerow" name="removerow"></a> removeRow

▪ `Static` **removeRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} removeRow - 移除一行

**`代码示例`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="resetrow" name="resetrow"></a> resetRow

▪ `Static` **resetRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} resetRow - 重置行的数据变化

**`代码示例`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="saverow" name="saverow"></a> saveRow

▪ `Static` **saveRow**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} saveRow - 保存行中的数据变化

**`代码示例`**
```
let buildInRowActions = GC.Spread.Sheets.TableSheet.BuiltInRowActions;
let options = tableSheet.rowActionOptions();
tableSheet.rowActionOptions(options.concat([buildInRowActions.removeRow,buildInRowActions.saveRow,buildInRowActions.resetRow]));
```

___

### <a id="warninginfo" name="warninginfo"></a> warningInfo

▪ `Static` **warningInfo**: [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)

集算表中内置的行操作

**`property`** {GC.Spread.Sheets.TableSheet.IRowActionOptions} warningInfo - 在行中显示警告信息
