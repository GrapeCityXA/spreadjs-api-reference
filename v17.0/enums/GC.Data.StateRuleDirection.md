# Enumeration: StateRuleDirection

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).StateRuleDirection

定义样式规则的应用方向

**`代码示例`**
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

样式规则将同时应用于行和列的方向

___

### <a id="column" name="column"></a> column

• **column** = `2`

样式规则将应用于列的方向

___

### <a id="none" name="none"></a> none

• **none** = `0`

样式规则将不被应用

___

### <a id="row" name="row"></a> row

• **row** = `1`

样式规则将应用于行的方向
