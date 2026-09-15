# Enumeration: DataOrientation

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).DataOrientation

区域的方向

**`代码示例`**
``` javascript
//本示例使用DataOrientation枚举
activeSheet.setValue(0, 0, "Data Range is A2-A9");
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
var s1=  activeSheet.setSparkline(11, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
var s2 =activeSheet.setSparkline(11, 3, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.column, setting);
var s3=  activeSheet.setSparkline(11, 6, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.winloss, setting);
var group = activeSheet.groupSparkline([s1,s2,s3]);
```

## Table of contents

### Enumeration members

- [horizontal](GC.Spread.Sheets.Sparklines.DataOrientation.md#horizontal)
- [vertical](GC.Spread.Sheets.Sparklines.DataOrientation.md#vertical)

## Enumeration members

### <a id="horizontal" name="horizontal"></a> horizontal

• **horizontal** = `1`

水平方向

___

### <a id="vertical" name="vertical"></a> vertical

• **vertical** = `0`

垂直方向
