# Enumeration: StateRuleDirection

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).StateRuleDirection

定义样式规则应用的方向。

**`example`**
```
view.addStyleRule("hoverRowStyle", GC.Data.View.StateRuleDirection, { backColor: "green" }, { state: GC.Data.RowColumnStates.hover });
```

## Table of contents

### Enumeration members

- [both](GC.Data.StateRuleDirection.md#both)
- [column](GC.Data.StateRuleDirection.md#column)
- [none](GC.Data.StateRuleDirection.md#none)
- [row](GC.Data.StateRuleDirection.md#row)

## Enumeration members

### <a id="both" name="both"></a> both

• **both** = `3`

指定样式规则将同时应用于行和列方向。

___

### <a id="column" name="column"></a> column

• **column** = `2`

指定样式规则将应用于列方向。

___

### <a id="none" name="none"></a> none

• **none** = `0`

指定不应用样式规则。

___

### <a id="row" name="row"></a> row

• **row** = `1`

指定样式规则将应用于行方向。
