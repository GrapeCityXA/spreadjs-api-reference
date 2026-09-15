# Enumeration: OutlineState

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).OutlineState

区域分组的状态

**`代码示例`**
```
//以下示例指定将区域分组显示为折叠状态
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

用加号指示折叠状态

___

### <a id="expanded" name="expanded"></a> expanded

• **expanded** = `0`

用减号指示扩展状态
