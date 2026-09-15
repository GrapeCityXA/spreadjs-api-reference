# Interface: IGroupByOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IGroupByOptions

## Hierarchy

- [`IGroupColumnOptions`](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md)

  ↳ **`IGroupByOptions`**

## Table of contents

### Properties

- [allowFilterByList](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#allowfilterbylist)
- [allowFilterByValue](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#allowfilterbyvalue)
- [allowSort](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#allowsort)
- [caption](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#caption)
- [conditionalFormats](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#conditionalformats)
- [field](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#field)
- [headerFit](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#headerfit)
- [headerStyle](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#headerstyle)
- [showEmptyAs](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#showemptyas)
- [showNullAs](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#shownullas)
- [spacing](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#spacing)
- [style](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#style)
- [summaryFields](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#summaryfields)
- [validator](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#validator)
- [width](GC.Spread.Sheets.TableSheet.IGroupByOptions.md#width)

## Properties

### <a id="allowfilterbylist" name="allowfilterbylist"></a> allowFilterByList

• `Optional` **allowFilterByList**: `boolean`

打开筛选对话框后是否显示按列表筛选。如果allowSort、allowFilterByValue和allowFilterByList都为false，则不显示该列的筛选按钮

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[allowFilterByList](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowfilterbylist)

___

### <a id="allowfilterbyvalue" name="allowfilterbyvalue"></a> allowFilterByValue

• `Optional` **allowFilterByValue**: `boolean`

打开筛选对话框后是否显示按值筛选

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[allowFilterByValue](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowfilterbyvalue)

___

### <a id="allowsort" name="allowsort"></a> allowSort

• `Optional` **allowSort**: `boolean`

打开筛选对话框后是否显示排序

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[allowSort](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#allowsort)

___

### <a id="caption" name="caption"></a> caption

• `Optional` **caption**: `string`

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[caption](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#caption)

___

### <a id="conditionalformats" name="conditionalformats"></a> conditionalFormats

• `Optional` **conditionalFormats**: ([`AverageRuleOptions`](../modules/GC.Data.md#averageruleoptions) \| [`CellValueRuleOptions`](../modules/GC.Data.md#cellvalueruleoptions) \| [`DataBarRuleOptions`](../modules/GC.Data.md#databarruleoptions) \| [`DateOccurringRuleOptions`](../modules/GC.Data.md#dateoccurringruleoptions) \| [`DuplicateRuleOptions`](../modules/GC.Data.md#duplicateruleoptions) \| [`FormulaRuleOptions`](../modules/GC.Data.md#formularuleoptions) \| [`SpecificTextRuleOptions`](../modules/GC.Data.md#specifictextruleoptions) \| [`Top10RuleOptions`](../modules/GC.Data.md#top10ruleoptions) \| [`UniqueRuleOptions`](../modules/GC.Data.md#uniqueruleoptions) \| [`TwoScaleRuleOptions`](../modules/GC.Data.md#twoscaleruleoptions) \| [`ThreeScaleRuleOptions`](../modules/GC.Data.md#threescaleruleoptions) \| [`IconSetRuleOptions`](../modules/GC.Data.md#iconsetruleoptions) \| [`SparklineRuleOptions`](../modules/GC.Data.md#sparklineruleoptions))[]

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[conditionalFormats](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#conditionalformats)

___

### <a id="field" name="field"></a> field

• **field**: `string`

___

### <a id="headerfit" name="headerfit"></a> headerFit

• `Optional` **headerFit**: ``"normal"`` \| ``"vertical"`` \| ``"stack"``

标题适应模式，默认为normal

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[headerFit](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerfit)

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

• `Optional` **headerStyle**: [`HeaderStyleOptions`](../modules/GC.Data.md#headerstyleoptions)

列标题样式

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[headerStyle](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerstyle)

___

### <a id="showemptyas" name="showemptyas"></a> showEmptyAs

• `Optional` **showEmptyAs**: `string`

空字符串值的显示文本。

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[showEmptyAs](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#showemptyas)

___

### <a id="shownullas" name="shownullas"></a> showNullAs

• `Optional` **showNullAs**: `string`

null 或 undefined 值的显示文本。

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[showNullAs](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#shownullas)

___

### <a id="spacing" name="spacing"></a> spacing

• `Optional` **spacing**: [`IGroupSpacingOptions`](GC.Spread.Sheets.TableSheet.IGroupSpacingOptions.md)

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`StyleOptions`](../modules/GC.Data.md#styleoptions)

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[style](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#style)

___

### <a id="summaryfields" name="summaryfields"></a> summaryFields

• `Optional` **summaryFields**: [`IGroupSummaryFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md)[]

___

### <a id="validator" name="validator"></a> validator

• `Optional` **validator**: [`DateValidatorOptions`](../modules/GC.Data.md#datevalidatoroptions) \| [`FormulaListValidatorOptions`](../modules/GC.Data.md#formulalistvalidatoroptions) \| [`FormulaValidatorOptions`](../modules/GC.Data.md#formulavalidatoroptions) \| [`NumberValidatorOptions`](../modules/GC.Data.md#numbervalidatoroptions) \| [`TimeValidatorOptions`](../modules/GC.Data.md#timevalidatoroptions) \| [`TextLengthValidatorOptions`](../modules/GC.Data.md#textlengthvalidatoroptions) \| [`ListValidatorOptions`](../modules/GC.Data.md#listvalidatoroptions)

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[validator](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#validator)

___

### <a id="width" name="width"></a> width

• `Optional` **width**: `number`

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[width](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#width)
