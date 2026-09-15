# Interface: IDeserializationOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IDeserializationOptions

## Table of contents

### Properties

- [doNotRecalculateAfterLoad](GC.Spread.Sheets.IDeserializationOptions.md#donotrecalculateafterload)
- [frozenColumnsAsRowHeaders](GC.Spread.Sheets.IDeserializationOptions.md#frozencolumnsasrowheaders)
- [frozenRowsAsColumnHeaders](GC.Spread.Sheets.IDeserializationOptions.md#frozenrowsascolumnheaders)
- [ignoreFormula](GC.Spread.Sheets.IDeserializationOptions.md#ignoreformula)
- [ignoreStyle](GC.Spread.Sheets.IDeserializationOptions.md#ignorestyle)
- [incrementalLoading](GC.Spread.Sheets.IDeserializationOptions.md#incrementalloading)

## Properties

### <a id="donotrecalculateafterload" name="donotrecalculateafterload"></a> doNotRecalculateAfterLoad

• `Optional` **doNotRecalculateAfterLoad**: `boolean`

是否在加载 json 数据后不重新计算。

___

### <a id="frozencolumnsasrowheaders" name="frozencolumnsasrowheaders"></a> frozenColumnsAsRowHeaders

• `Optional` **frozenColumnsAsRowHeaders**: `boolean`

是否在将 json 转换为工作簿时将冻结的列视为行标题。

___

### <a id="frozenrowsascolumnheaders" name="frozenrowsascolumnheaders"></a> frozenRowsAsColumnHeaders

• `Optional` **frozenRowsAsColumnHeaders**: `boolean`

是否在将 json 转换为工作簿时将冻结的行视为列标题。

___

### <a id="ignoreformula" name="ignoreformula"></a> ignoreFormula

• `Optional` **ignoreFormula**: `boolean`

是否在将 json 转换为工作簿时忽略公式。

___

### <a id="ignorestyle" name="ignorestyle"></a> ignoreStyle

• `Optional` **ignoreStyle**: `boolean`

是否在将 json 转换为工作簿时忽略样式。

___

### <a id="incrementalloading" name="incrementalloading"></a> incrementalLoading

• `Optional` **incrementalLoading**: `boolean` \| [`IIncrementalLoadingOptions`](GC.Spread.Sheets.IIncrementalLoadingOptions.md)

是否在将 json 转换为工作簿时使用增量加载或增量加载的回调。
