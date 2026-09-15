# Interface: ITableSheetOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).ITableSheetOptions

## Table of contents

### Properties

- [allowAddNew](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#allowaddnew)
- [allowSorts](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#allowsorts)
- [alternatingRowOptions](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#alternatingrowoptions)
- [columnTypeItems](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#columntypeitems)
- [defaultStackRowHeight](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#defaultstackrowheight)
- [defineColumnCommand](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#definecolumncommand)
- [enableDefineColumn](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#enabledefinecolumn)
- [groupLayout](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#grouplayout)
- [menuItemVisibility](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#menuitemvisibility)
- [sheetTabColor](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#sheettabcolor)
- [showRowNumber](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#showrownumber)
- [submitDefineColumnCommand](GC.Spread.Sheets.TableSheet.ITableSheetOptions.md#submitdefinecolumncommand)

## Properties

### <a id="allowaddnew" name="allowaddnew"></a> allowAddNew

• `Optional` **allowAddNew**: `boolean`

是否允许添加新的空行。

___

### <a id="allowsorts" name="allowsorts"></a> allowSorts

• `Optional` **allowSorts**: `boolean`

是否允许对多列进行排序。

___

### <a id="alternatingrowoptions" name="alternatingrowoptions"></a> alternatingRowOptions

• `Optional` **alternatingRowOptions**: [`IAlternatingRowOptions`](GC.Spread.Sheets.TableSheet.IAlternatingRowOptions.md)

定义交替行样式选项。

___

### <a id="columntypeitems" name="columntypeitems"></a> columnTypeItems

• `Optional` **columnTypeItems**: [`IColumnTypeItem`](GC.Spread.Sheets.TableSheet.IColumnTypeItem.md)[]

指定列类型。

___

### <a id="defaultstackrowheight" name="defaultstackrowheight"></a> defaultStackRowHeight

• `Optional` **defaultStackRowHeight**: `number`

表格默认堆叠行高，默认情况下将计算平均高度，默认值为null。

___

### <a id="definecolumncommand" name="definecolumncommand"></a> defineColumnCommand

• `Optional` **defineColumnCommand**: `string`

指定定义列选项的命令。

___

### <a id="enabledefinecolumn" name="enabledefinecolumn"></a> enableDefineColumn

• `Optional` **enableDefineColumn**: `boolean`

是否启用定义列。

___

### <a id="grouplayout" name="grouplayout"></a> groupLayout

• `Optional` **groupLayout**: [`IGroupLayoutOptions`](GC.Spread.Sheets.TableSheet.IGroupLayoutOptions.md)

指定分组布局的选项。

___

### <a id="menuitemvisibility" name="menuitemvisibility"></a> menuItemVisibility

• `Optional` **menuItemVisibility**: [`IMenuItemVisibility`](GC.Spread.Sheets.TableSheet.IMenuItemVisibility.md)

表格中菜单项的可见性。

___

### <a id="sheettabcolor" name="sheettabcolor"></a> sheetTabColor

• `Optional` **sheetTabColor**: `string`

用于表示工作表标签颜色的颜色字符串，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等。

___

### <a id="showrownumber" name="showrownumber"></a> showRowNumber

• `Optional` **showRowNumber**: `boolean`

是否显示行号标题。

___

### <a id="submitdefinecolumncommand" name="submitdefinecolumncommand"></a> submitDefineColumnCommand

• `Optional` **submitDefineColumnCommand**: `string`

指定提交已定义列选项的命令。
