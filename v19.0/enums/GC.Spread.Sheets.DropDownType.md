# Enumeration: DropDownType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).DropDownType

指定下拉类型。

**`example`**
```
//此示例设置下拉类型。
//创建样式
var style = new GC.Spread.Sheets.Style();
style.dropDowns=[
   {
     type:GC.Spread.Sheets.DropDownType.dateTimePicker,
     option: {
         showTime:false
     }
   }
];
sheet.setStyle(0, 0, style);
```

## Table of contents

### Enumeration members

- [calculator](GC.Spread.Sheets.DropDownType.md#calculator)
- [colorPicker](GC.Spread.Sheets.DropDownType.md#colorpicker)
- [dateTimePicker](GC.Spread.Sheets.DropDownType.md#datetimepicker)
- [list](GC.Spread.Sheets.DropDownType.md#list)
- [monthPicker](GC.Spread.Sheets.DropDownType.md#monthpicker)
- [multiColumn](GC.Spread.Sheets.DropDownType.md#multicolumn)
- [slider](GC.Spread.Sheets.DropDownType.md#slider)
- [timePicker](GC.Spread.Sheets.DropDownType.md#timepicker)
- [workflowList](GC.Spread.Sheets.DropDownType.md#workflowlist)

## Enumeration members

### <a id="calculator" name="calculator"></a> calculator

• **calculator** = `6`

表示下拉类型为计算器。

___

### <a id="colorpicker" name="colorpicker"></a> colorPicker

• **colorPicker** = `0`

表示下拉类型为颜色选择器。

___

### <a id="datetimepicker" name="datetimepicker"></a> dateTimePicker

• **dateTimePicker** = `1`

表示下拉类型为日期时间选择器。

___

### <a id="list" name="list"></a> list

• **list** = `4`

表示下拉类型为列表。

___

### <a id="monthpicker" name="monthpicker"></a> monthPicker

• **monthPicker** = `3`

表示下拉类型为月份选择器。

___

### <a id="multicolumn" name="multicolumn"></a> multiColumn

• **multiColumn** = `8`

表示下拉类型为多列。

___

### <a id="slider" name="slider"></a> slider

• **slider** = `5`

表示下拉类型为滑块。

___

### <a id="timepicker" name="timepicker"></a> timePicker

• **timePicker** = `2`

表示下拉类型为时间选择器。

___

### <a id="workflowlist" name="workflowlist"></a> workflowList

• **workflowList** = `7`

表示下拉类型为工作流列表。
