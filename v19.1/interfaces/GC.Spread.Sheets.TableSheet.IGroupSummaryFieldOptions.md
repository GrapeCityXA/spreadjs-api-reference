# Interface: IGroupSummaryFieldOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IGroupSummaryFieldOptions

## Hierarchy

- [`IGroupColumnOptions`](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md)

  ↳ **`IGroupSummaryFieldOptions`**

## Table of contents

### Properties

- [allowFilterByList](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#allowfilterbylist)
- [allowFilterByValue](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#allowfilterbyvalue)
- [allowSort](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#allowsort)
- [caption](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#caption)
- [conditionalFormats](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#conditionalformats)
- [formula](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#formula)
- [headerFit](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#headerfit)
- [headerStyle](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#headerstyle)
- [position](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#position)
- [relateTo](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#relateto)
- [showEmptyAs](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#showemptyas)
- [showNullAs](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#shownullas)
- [slice](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#slice)
- [style](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#style)
- [validator](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#validator)
- [width](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md#width)

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

### <a id="formula" name="formula"></a> formula

• **formula**: `string`

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

### <a id="position" name="position"></a> position

• `Optional` **position**: ``"header"`` \| ``"footer"``

___

### <a id="relateto" name="relateto"></a> relateTo

• `Optional` **relateTo**: `string`

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

### <a id="slice" name="slice"></a> slice

• `Optional` **slice**: `string` \| [`IGroupSummarySliceFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummarySliceFieldOptions.md)

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`StyleOptions`](../modules/GC.Data.md#styleoptions)

#### Inherited from

[IGroupColumnOptions](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md).[style](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#style)

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
