# Enumeration: FillDateUnit

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).FillDateUnit

日期填充单位

**`代码示例`**
```
//本示例使用FillDateUnit枚举
spread.options.allowUserDragFill = true;
activeSheet.setValue(0, 0, new Date(2011, 1, 1));
activeSheet.setValue(0, 1, new Date(2011, 2, 9));
activeSheet.setValue(0, 2, 5);
activeSheet.setValue(0, 3, 10);
activeSheet.setValue(0, 4, 1);

var start = new GC.Spread.Sheets.Range(0, 0, 1, 1);
var r = new GC.Spread.Sheets.Range(0, 0, 4, 1);
activeSheet.fillAuto(start, r, {
    fillType: GC.Spread.Sheets.Fill.FillType.date,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
    fillDirection: GC.Spread.Sheets.Fill.FillDirection.down,
    unit: GC.Spread.Sheets.Fill.FillDateUnit.day,
    step: 1,
    stop: new Date(2011, 2, 11)
});

start = new GC.Spread.Sheets.Range(0, 1, 1, 1);
var r2 = new GC.Spread.Sheets.Range(0, 1, 4, 1);
activeSheet.fillAuto(start, r2, {
fillType: GC.Spread.Sheets.Fill.FillType.date,
series: GC.Spread.Sheets.Fill.FillSeries.column,
fillDirection:GC.Spread.Sheets.Fill.FillDirection.down,
unit: GC.Spread.Sheets.Fill.FillDateUnit.day,
step: 1,
stop: new Date(2011, 2, 11)
});

start = new GC.Spread.Sheets.Range(0, 2, 1, 1);
var r3 = new GC.Spread.Sheets.Range(0, 2, 4, 1);
activeSheet.fillAuto(start, r3, {
    fillType: GC.Spread.Sheets.Fill.FillType.auto,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
});

start = new GC.Spread.Sheets.Range(0, 3, 1, 1);
var r4 = new GC.Spread.Sheets.Range(0, 3, 4, 1);
activeSheet.fillAuto(start, r4, {
    fillType: GC.Spread.Sheets.Fill.FillType.growth,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
    step:2,
    stop:55
});

start = new GC.Spread.Sheets.Range(0, 4, 1, 1);
var r5 = new GC.Spread.Sheets.Range(0, 4, 4, 1);
activeSheet.fillAuto(start, r5, {
    fillType: GC.Spread.Sheets.Fill.FillType.linear,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
    step:3,
    stop:20
});

activeSheet.setValue(0, 5, 123);
var r6 = new GC.Spread.Sheets.Range(0, 5, 4, 1);
activeSheet.fillAuto(new GC.Spread.Sheets.Range(0, 5, 1, 1), r6, {
    fillType: GC.Spread.Sheets.Fill.FillType.auto,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
});
```

## Table of contents

### Enumeration members

- [day](GC.Spread.Sheets.Fill.FillDateUnit.md#day)
- [month](GC.Spread.Sheets.Fill.FillDateUnit.md#month)
- [weekday](GC.Spread.Sheets.Fill.FillDateUnit.md#weekday)
- [year](GC.Spread.Sheets.Fill.FillDateUnit.md#year)

## Enumeration members

### <a id="day" name="day"></a> day

• **day** = `0`

将日期填充单位设置为天

___

### <a id="month" name="month"></a> month

• **month** = `2`

将日期填充单位设置为月

___

### <a id="weekday" name="weekday"></a> weekday

• **weekday** = `1`

将日期填充单位设置为周

___

### <a id="year" name="year"></a> year

• **year** = `3`

将日期填充单位设置为年
