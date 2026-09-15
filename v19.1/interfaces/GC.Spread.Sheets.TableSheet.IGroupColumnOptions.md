# Interface: IGroupColumnOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IGroupColumnOptions

## Hierarchy

- **`IGroupColumnOptions`**

  ↳ [`IGroupByOptions`](GC.Spread.Sheets.TableSheet.IGroupByOptions.md)

  ↳ [`IGroupSummaryFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md)

  ↳ [`IGroupSummarySliceFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummarySliceFieldOptions.md)

## Table of contents

### Properties

- [allowFilterByList](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowfilterbylist)
- [allowFilterByValue](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowfilterbyvalue)
- [allowSort](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowsort)
- [caption](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#caption)
- [conditionalFormats](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#conditionalformats)
- [headerFit](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerfit)
- [headerStyle](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerstyle)
- [showEmptyAs](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#showemptyas)
- [showNullAs](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#shownullas)
- [style](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#style)
- [validator](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#validator)
- [width](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#width)

## Properties

### <a id="allowfilterbylist" name="allowfilterbylist"></a> allowFilterByList

• `Optional` **allowFilterByList**: `boolean`

打开筛选对话框后是否显示按列表筛选。如果allowSort、allowFilterByValue和allowFilterByList都为false，则不显示该列的筛选按钮

___

### <a id="allowfilterbyvalue" name="allowfilterbyvalue"></a> allowFilterByValue

• `Optional` **allowFilterByValue**: `boolean`

打开筛选对话框后是否显示按值筛选

___

### <a id="allowsort" name="allowsort"></a> allowSort

• `Optional` **allowSort**: `boolean`

打开筛选对话框后是否显示排序

___

### <a id="caption" name="caption"></a> caption

• `Optional` **caption**: `string`

___

### <a id="conditionalformats" name="conditionalformats"></a> conditionalFormats

• `Optional` **conditionalFormats**: ([`AverageRuleOptions`](../modules/GC.Data.md#averageruleoptions) \| [`CellValueRuleOptions`](../modules/GC.Data.md#cellvalueruleoptions) \| [`DataBarRuleOptions`](../modules/GC.Data.md#databarruleoptions) \| [`DateOccurringRuleOptions`](../modules/GC.Data.md#dateoccurringruleoptions) \| [`DuplicateRuleOptions`](../modules/GC.Data.md#duplicateruleoptions) \| [`FormulaRuleOptions`](../modules/GC.Data.md#formularuleoptions) \| [`SpecificTextRuleOptions`](../modules/GC.Data.md#specifictextruleoptions) \| [`Top10RuleOptions`](../modules/GC.Data.md#top10ruleoptions) \| [`UniqueRuleOptions`](../modules/GC.Data.md#uniqueruleoptions) \| [`TwoScaleRuleOptions`](../modules/GC.Data.md#twoscaleruleoptions) \| [`ThreeScaleRuleOptions`](../modules/GC.Data.md#threescaleruleoptions) \| [`IconSetRuleOptions`](../modules/GC.Data.md#iconsetruleoptions) \| [`SparklineRuleOptions`](../modules/GC.Data.md#sparklineruleoptions))[]

___

### <a id="headerfit" name="headerfit"></a> headerFit

• `Optional` **headerFit**: ``"normal"`` \| ``"vertical"`` \| ``"stack"``

标题适应模式，默认为normal

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

• `Optional` **headerStyle**: [`HeaderStyleOptions`](../modules/GC.Data.md#headerstyleoptions)

列标题样式

___

### <a id="showemptyas" name="showemptyas"></a> showEmptyAs

• `Optional` **showEmptyAs**: `string`

空字符串值的显示文本。

___

### <a id="shownullas" name="shownullas"></a> showNullAs

• `Optional` **showNullAs**: `string`

null 或 undefined 值的显示文本。

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`StyleOptions`](../modules/GC.Data.md#styleoptions)

___

### <a id="validator" name="validator"></a> validator

• `Optional` **validator**: [`DateValidatorOptions`](../modules/GC.Data.md#datevalidatoroptions) \| [`FormulaListValidatorOptions`](../modules/GC.Data.md#formulalistvalidatoroptions) \| [`FormulaValidatorOptions`](../modules/GC.Data.md#formulavalidatoroptions) \| [`NumberValidatorOptions`](../modules/GC.Data.md#numbervalidatoroptions) \| [`TimeValidatorOptions`](../modules/GC.Data.md#timevalidatoroptions) \| [`TextLengthValidatorOptions`](../modules/GC.Data.md#textlengthvalidatoroptions) \| [`ListValidatorOptions`](../modules/GC.Data.md#listvalidatoroptions)

___

### <a id="width" name="width"></a> width

• `Optional` **width**: `number`
