# Enumeration: IconSetType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).IconSetType

指定图标集。

**`example`**
```
//此示例创建规则。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
var iconCriteria = iconSetRule.iconCriteria();
iconCriteria[0] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 1);
iconCriteria[1] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 10);
iconCriteria[2] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 20);
iconSetRule.iconCriteria(iconCriteria);
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

## Table of contents

### Enumeration members

- [fiveArrowsColored](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fivearrowscolored)
- [fiveArrowsGray](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fivearrowsgray)
- [fiveBoxes](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fiveboxes)
- [fiveQuarters](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fivequarters)
- [fiveRatings](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fiveratings)
- [fourArrowsColored](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fourarrowscolored)
- [fourArrowsGray](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fourarrowsgray)
- [fourRatings](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fourratings)
- [fourRedToBlack](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fourredtoblack)
- [fourTrafficLights](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#fourtrafficlights)
- [noIcons](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#noicons)
- [threeArrowsColored](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threearrowscolored)
- [threeArrowsGray](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threearrowsgray)
- [threeFlags](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threeflags)
- [threeSigns](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threesigns)
- [threeStars](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threestars)
- [threeSymbolsCircled](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threesymbolscircled)
- [threeSymbolsUncircled](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threesymbolsuncircled)
- [threeTrafficLightsRimmed](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threetrafficlightsrimmed)
- [threeTrafficLightsUnrimmed](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threetrafficlightsunrimmed)
- [threeTriangles](GC.Spread.Sheets.ConditionalFormatting.IconSetType.md#threetriangles)

## Enumeration members

### <a id="fivearrowscolored" name="fivearrowscolored"></a> fiveArrowsColored

• **fiveArrowsColored** = `15`

指定五个彩色箭头。

___

### <a id="fivearrowsgray" name="fivearrowsgray"></a> fiveArrowsGray

• **fiveArrowsGray** = `16`

指定五个灰色箭头。

___

### <a id="fiveboxes" name="fiveboxes"></a> fiveBoxes

• **fiveBoxes** = `19`

指定五个方框。

___

### <a id="fivequarters" name="fivequarters"></a> fiveQuarters

• **fiveQuarters** = `18`

指定五个四分之一。

___

### <a id="fiveratings" name="fiveratings"></a> fiveRatings

• **fiveRatings** = `17`

指定五个评级。

___

### <a id="fourarrowscolored" name="fourarrowscolored"></a> fourArrowsColored

• **fourArrowsColored** = `10`

指定四个彩色箭头。

___

### <a id="fourarrowsgray" name="fourarrowsgray"></a> fourArrowsGray

• **fourArrowsGray** = `11`

指定四个灰色箭头。

___

### <a id="fourratings" name="fourratings"></a> fourRatings

• **fourRatings** = `13`

指定四个评级。

___

### <a id="fourredtoblack" name="fourredtoblack"></a> fourRedToBlack

• **fourRedToBlack** = `12`

指定四个红到黑图标。

___

### <a id="fourtrafficlights" name="fourtrafficlights"></a> fourTrafficLights

• **fourTrafficLights** = `14`

指定四个交通灯。

___

### <a id="noicons" name="noicons"></a> noIcons

• **noIcons** = `20`

指定无单元格图标。

___

### <a id="threearrowscolored" name="threearrowscolored"></a> threeArrowsColored

• **threeArrowsColored** = `0`

指定三个彩色箭头。

___

### <a id="threearrowsgray" name="threearrowsgray"></a> threeArrowsGray

• **threeArrowsGray** = `1`

指定三个灰色箭头。

___

### <a id="threeflags" name="threeflags"></a> threeFlags

• **threeFlags** = `4`

指定三个旗帜。

___

### <a id="threesigns" name="threesigns"></a> threeSigns

• **threeSigns** = `7`

指定三个符号。

___

### <a id="threestars" name="threestars"></a> threeStars

• **threeStars** = `3`

指定三个星形。

___

### <a id="threesymbolscircled" name="threesymbolscircled"></a> threeSymbolsCircled

• **threeSymbolsCircled** = `8`

指定三个符号（带圆圈）。

___

### <a id="threesymbolsuncircled" name="threesymbolsuncircled"></a> threeSymbolsUncircled

• **threeSymbolsUncircled** = `9`

指定三个符号（无圆圈）。

___

### <a id="threetrafficlightsrimmed" name="threetrafficlightsrimmed"></a> threeTrafficLightsRimmed

• **threeTrafficLightsRimmed** = `6`

指定三个交通灯（有边框）。

___

### <a id="threetrafficlightsunrimmed" name="threetrafficlightsunrimmed"></a> threeTrafficLightsUnrimmed

• **threeTrafficLightsUnrimmed** = `5`

指定三个交通灯（无边框）。

___

### <a id="threetriangles" name="threetriangles"></a> threeTriangles

• **threeTriangles** = `2`

指定三个三角形。
