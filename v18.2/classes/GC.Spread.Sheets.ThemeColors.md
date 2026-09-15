# Class: ThemeColors

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ThemeColors

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ThemeColors.md#constructor)

### Properties

- [Apex](GC.Spread.Sheets.ThemeColors.md#apex)
- [Aspect](GC.Spread.Sheets.ThemeColors.md#aspect)
- [Civic](GC.Spread.Sheets.ThemeColors.md#civic)
- [Concourse](GC.Spread.Sheets.ThemeColors.md#concourse)
- [Default](GC.Spread.Sheets.ThemeColors.md#default)
- [Equity](GC.Spread.Sheets.ThemeColors.md#equity)
- [Flow](GC.Spread.Sheets.ThemeColors.md#flow)
- [Foundry](GC.Spread.Sheets.ThemeColors.md#foundry)
- [Median](GC.Spread.Sheets.ThemeColors.md#median)
- [Metro](GC.Spread.Sheets.ThemeColors.md#metro)
- [Module](GC.Spread.Sheets.ThemeColors.md#module)
- [Office](GC.Spread.Sheets.ThemeColors.md#office)
- [Office2007](GC.Spread.Sheets.ThemeColors.md#office2007)
- [Opulent](GC.Spread.Sheets.ThemeColors.md#opulent)
- [Oriel](GC.Spread.Sheets.ThemeColors.md#oriel)
- [Origin](GC.Spread.Sheets.ThemeColors.md#origin)
- [Paper](GC.Spread.Sheets.ThemeColors.md#paper)
- [Solstice](GC.Spread.Sheets.ThemeColors.md#solstice)
- [Technic](GC.Spread.Sheets.ThemeColors.md#technic)
- [Trek](GC.Spread.Sheets.ThemeColors.md#trek)
- [Urban](GC.Spread.Sheets.ThemeColors.md#urban)
- [Verve](GC.Spread.Sheets.ThemeColors.md#verve)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ThemeColors**()

表示内置主题的颜色。

**`example`**
```
//此示例创建一个自定义主题。
var custom = new GC.Spread.Sheets.Theme("CustomTheme");
custom.colors().accent1("red");
custom.colors().accent6("green");
custom.colors().textColor1("orange");
activeSheet.currentTheme(custom);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 1 30");
```

## Properties

### <a id="apex" name="apex"></a> Apex

• **Apex**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

表示Apex主题的颜色。

**`example`**
```
//此示例使用Apex主题。
activeSheet.currentTheme("Apex");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="aspect" name="aspect"></a> Aspect

• **Aspect**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Aspect主题的颜色。

**`example`**
```
//此示例使用Aspect主题。
activeSheet.currentTheme("Aspect");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="civic" name="civic"></a> Civic

• **Civic**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Civic主题的颜色。

**`example`**
```
//此示例使用Civic主题。
activeSheet.currentTheme("Civic");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="concourse" name="concourse"></a> Concourse

• **Concourse**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Concourse主题的颜色。

**`example`**
```
//此示例使用Concourse主题。
activeSheet.currentTheme("Concourse");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="default" name="default"></a> Default

• **Default**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Default主题的颜色。

**`example`**
```
//此示例设置Default主题。
activeSheet.currentTheme("Default");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="equity" name="equity"></a> Equity

• **Equity**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Equity主题的颜色。

**`example`**
```
//此示例设置Equity主题。
activeSheet.currentTheme("Equity");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="flow" name="flow"></a> Flow

• **Flow**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Flow主题的颜色。

**`example`**
```
//此示例设置Flow主题。
activeSheet.currentTheme("Flow");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="foundry" name="foundry"></a> Foundry

• **Foundry**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Foundry主题的颜色。

**`example`**
```
//此示例设置Foundry主题。
activeSheet.currentTheme("Foundry");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="median" name="median"></a> Median

• **Median**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Median主题的颜色。

**`example`**
```
//此示例设置Median主题。
activeSheet.currentTheme("Median");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="metro" name="metro"></a> Metro

• **Metro**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Metro主题的颜色。

**`example`**
```
//此示例设置Metro主题。
activeSheet.currentTheme("Metro");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="module" name="module"></a> Module

• **Module**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Module主题的颜色。

**`example`**
```
//此示例设置Module主题。
activeSheet.currentTheme("Module");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="office" name="office"></a> Office

• **Office**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Office主题的颜色。

**`example`**
```
//此示例设置Office主题。
activeSheet.currentTheme("Office");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="office2007" name="office2007"></a> Office2007

• **Office2007**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Office 2007主题的颜色。

**`example`**
```
//此示例使用Office2007主题。
activeSheet.currentTheme("Office2007");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="opulent" name="opulent"></a> Opulent

• **Opulent**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Opulent主题的颜色。

**`example`**
```
//此示例设置Opulent主题。
activeSheet.currentTheme("Opulent");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="oriel" name="oriel"></a> Oriel

• **Oriel**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Oriel主题的颜色。

**`example`**
```
//此示例设置Oriel主题。
activeSheet.currentTheme("Oriel");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="origin" name="origin"></a> Origin

• **Origin**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Origin主题的颜色。

**`example`**
```
//此示例设置Origin主题。
activeSheet.currentTheme("Origin");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="paper" name="paper"></a> Paper

• **Paper**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Paper主题的颜色。

**`example`**
```
//此示例设置Paper主题。
activeSheet.currentTheme("Paper");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="solstice" name="solstice"></a> Solstice

• **Solstice**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Solstice主题的颜色。

**`example`**
```
//此示例设置Solstice主题。
activeSheet.currentTheme("Solstice");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="technic" name="technic"></a> Technic

• **Technic**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Technic主题的颜色。

**`example`**
```
//此示例设置Technic主题。
activeSheet.currentTheme("Technic");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="trek" name="trek"></a> Trek

• **Trek**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Trek主题的颜色。

**`example`**
```
//此示例设置Trek主题。
activeSheet.currentTheme("Trek");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="urban" name="urban"></a> Urban

• **Urban**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Urban主题的颜色。

**`example`**
```
//此示例设置Urban主题。
activeSheet.currentTheme("Urban");
activeSheet.resumePaint();
activeSheet.repaint();
```

___

### <a id="verve" name="verve"></a> Verve

• **Verve**: [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md)

Verve主题的颜色。

**`example`**
```
//此示例设置Verve主题。
activeSheet.currentTheme("Verve");
activeSheet.resumePaint();
activeSheet.repaint();
```
