# Enumeration: OutlineState

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).OutlineState

指定大纲（范围组）的状态。

**`example`**
```
//以下示例指定将范围组显示为折叠状态。
sheet.rowOutlines.group(0,5);
var rgi = sheet.rowOutlines.find(1, 0);
rgi.state(GC.Spread.Sheets.Outlines.OutlineState.collapsed);
spread.invalidateLayout();
spread.repaint();
```

## Table of contents

### Enumeration members

- [collapsed](GC.Spread.Sheets.Outlines.OutlineState.md#collapsed)
- [expanded](GC.Spread.Sheets.Outlines.OutlineState.md#expanded)

## Enumeration members

### <a id="collapsed" name="collapsed"></a> collapsed

• **collapsed** = `1`

表示折叠状态，使用加号标记。

___

### <a id="expanded" name="expanded"></a> expanded

• **expanded** = `0`

表示展开状态，使用减号标记。
