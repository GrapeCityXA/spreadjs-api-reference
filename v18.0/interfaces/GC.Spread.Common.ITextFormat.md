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

指定字符可以拆分两行。默认值为[“”，“  - ”]

___

### <a id="linebreakingforbidend" name="linebreakingforbidend"></a> lineBreakingForbidEnd

• `Optional` **lineBreakingForbidEnd**: `string`[]

指定在断行结束时不允许的字符

___

### <a id="linebreakingforbidstart" name="linebreakingforbidstart"></a> lineBreakingForbidStart

• `Optional` **lineBreakingForbidStart**: `string`[]

指定在断行开始时不允许的字符

___

### <a id="linebreakingstrategy" name="linebreakingstrategy"></a> lineBreakingStrategy

• `Optional` **lineBreakingStrategy**: [`ILineBreakingStrategy`](GC.Spread.Common.ILineBreakingStrategy.md)

指定单词拆分函数
