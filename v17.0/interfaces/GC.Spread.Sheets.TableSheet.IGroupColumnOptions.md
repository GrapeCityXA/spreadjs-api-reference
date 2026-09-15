# Interface: IGroupColumnOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IGroupColumnOptions

## Hierarchy

- **`IGroupColumnOptions`**

  ↳ [`IGroupByOptions`](GC.Spread.Sheets.TableSheet.IGroupByOptions.md)

  ↳ [`IGroupSummaryFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummaryFieldOptions.md)

  ↳ [`IGroupSummarySliceFieldOptions`](GC.Spread.Sheets.TableSheet.IGroupSummarySliceFieldOptions.md)

## Table of contents

### Properties

- [caption](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#caption)
- [conditionalFormats](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#conditionalformats)
- [headerFit](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerfit)
- [headerStyle](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#headerstyle)
- [style](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#style)
- [validator](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#validator)
- [width](GC.Spread.Sheets.TableSheet.IGroupColumnOptions.md#width)

## Properties

### <a id="caption" name="caption"></a> caption

• `Optional` **caption**: `string`

___

### <a id="conditionalformats" name="conditionalformats"></a> conditionalFormats

• `Optional` **conditionalFormats**: ([`AverageRuleOptions`](../modules/GC.Data.md#averageruleoptions) \| [`CellValueRuleOptions`](../modules/GC.Data.md#cellvalueruleoptions) \| [`DataBarRuleOptions`](../modules/GC.Data.md#databarruleoptions) \| [`DateOccurringRuleOptions`](../modules/GC.Data.md#dateoccurringruleoptions) \| [`DuplicateRuleOptions`](../modules/GC.Data.md#duplicateruleoptions) \| [`FormulaRuleOptions`](../modules/GC.Data.md#formularuleoptions) \| [`SpecificTextRuleOptions`](../modules/GC.Data.md#specifictextruleoptions) \| [`Top10RuleOptions`](../modules/GC.Data.md#top10ruleoptions) \| [`UniqueRuleOptions`](../modules/GC.Data.md#uniqueruleoptions) \| [`TwoScaleRuleOptions`](../modules/GC.Data.md#twoscaleruleoptions) \| [`ThreeScaleRuleOptions`](../modules/GC.Data.md#threescaleruleoptions) \| [`IconSetRuleOptions`](../modules/GC.Data.md#iconsetruleoptions))[]

___

### <a id="headerfit" name="headerfit"></a> headerFit

• `Optional` **headerFit**: ``"vertical"`` \| ``"normal"`` \| ``"stack"``

the header fit mode, default is normal

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

• `Optional` **headerStyle**: [`HeaderStyleOptions`](../modules/GC.Data.md#headerstyleoptions)

the column header style

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`StyleOptions`](../modules/GC.Data.md#styleoptions)

___

### <a id="validator" name="validator"></a> validator

• `Optional` **validator**: [`DateValidatorOptions`](../modules/GC.Data.md#datevalidatoroptions) \| [`FormulaListValidatorOptions`](../modules/GC.Data.md#formulalistvalidatoroptions) \| [`FormulaValidatorOptions`](../modules/GC.Data.md#formulavalidatoroptions) \| [`NumberValidatorOptions`](../modules/GC.Data.md#numbervalidatoroptions) \| [`TimeValidatorOptions`](../modules/GC.Data.md#timevalidatoroptions) \| [`TextLengthValidatorOptions`](../modules/GC.Data.md#textlengthvalidatoroptions) \| [`ListValidatorOptions`](../modules/GC.Data.md#listvalidatoroptions)

___

### <a id="width" name="width"></a> width

• `Optional` **width**: `number`
