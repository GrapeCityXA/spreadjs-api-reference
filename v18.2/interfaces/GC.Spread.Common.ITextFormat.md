# Interface: ITextFormat

[Spread](../modules/GC.Spread.md).[Common](../modules/GC.Spread.Common.md).ITextFormat

## Table of contents

### Properties

- [lineBreakingChar](GC.Spread.Common.ITextFormat.md#linebreakingchar)
- [lineBreakingForbidEnd](GC.Spread.Common.ITextFormat.md#linebreakingforbidend)
- [lineBreakingForbidStart](GC.Spread.Common.ITextFormat.md#linebreakingforbidstart)
- [lineBreakingStrategy](GC.Spread.Common.ITextFormat.md#linebreakingstrategy)

## Properties

### <a id="linebreakingchar" name="linebreakingchar"></a> lineBreakingChar

• `Optional` **lineBreakingChar**: `string`[]

指定可以分割两行的字符。默认为[" ", "-"]。

___

### <a id="linebreakingforbidend" name="linebreakingforbidend"></a> lineBreakingForbidEnd

• `Optional` **lineBreakingForbidEnd**: `string`[]

指定不允许在断行结束处的字符。

___

### <a id="linebreakingforbidstart" name="linebreakingforbidstart"></a> lineBreakingForbidStart

• `Optional` **lineBreakingForbidStart**: `string`[]

指定不允许在断行开始处的字符。

___

### <a id="linebreakingstrategy" name="linebreakingstrategy"></a> lineBreakingStrategy

• `Optional` **lineBreakingStrategy**: [`ILineBreakingStrategy`](GC.Spread.Common.ILineBreakingStrategy.md)

指定用于单词分割的函数。
