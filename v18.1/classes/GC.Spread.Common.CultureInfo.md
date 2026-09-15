# Class: CultureInfo

[Spread](../modules/GC.Spread.md).[Common](../modules/GC.Spread.Common.md).CultureInfo

## Table of contents

### Constructors

- [constructor](GC.Spread.Common.CultureInfo.md#constructor)

### Properties

- [DateTimeFormat](GC.Spread.Common.CultureInfo.md#datetimeformat)
- [LocalNumberFormat](GC.Spread.Common.CultureInfo.md#localnumberformat)
- [NumberFormat](GC.Spread.Common.CultureInfo.md#numberformat)
- [TextFormat](GC.Spread.Common.CultureInfo.md#textformat)
- [displayName](GC.Spread.Common.CultureInfo.md#displayname)
- [equalCharacters](GC.Spread.Common.CultureInfo.md#equalcharacters)
- [fontScriptCode](GC.Spread.Common.CultureInfo.md#fontscriptcode)
- [id](GC.Spread.Common.CultureInfo.md#id)
- [predefinedFormats](GC.Spread.Common.CultureInfo.md#predefinedformats)

### Methods

- [name](GC.Spread.Common.CultureInfo.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CultureInfo**()

表示自定义文化类。成员变量可以被覆盖。

## Properties

### <a id="datetimeformat" name="datetimeformat"></a> DateTimeFormat

• **DateTimeFormat**: [`IDateTimeFormat`](../interfaces/GC.Spread.Common.IDateTimeFormat.md)

表示日期时间格式字段。

**`example`**
```
// This example creates a custom culture.
var myCulture = new GC.Spread.Common.CultureInfo();
myCulture.NumberFormat.currencySymbol = "\u20ac"
myCulture.NumberFormat.numberDecimalSeparator = ",";
myCulture.NumberFormat.numberGroupSeparator = ".";
myCulture.NumberFormat.arrayGroupSeparator = ";";
myCulture.NumberFormat.arrayListSeparator = "\\";
myCulture.NumberFormat.listSeparator = ";";
myCulture.DateTimeFormat.amDesignator = "";
myCulture.DateTimeFormat.pmDesignator = "";
myCulture.DateTimeFormat.abbreviatedMonthNames = ["Jan", "Feb", "Mrz", "Apr", "Mai", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dez", ""];
myCulture.DateTimeFormat.abbreviatedDayNames = ["So", "Mo", "Di", "Mi", "Do", "Fr", "Sa"];
myCulture.DateTimeFormat.abbreviatedMonthGenitiveNames = ["Jan", "Feb", "Mrz", "Apr", "Mai", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dez", ""];
myCulture.DateTimeFormat.dayNames = ["Sonntag", "Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag"];
myCulture.DateTimeFormat.fullDateTimePattern = "dddd, d. MMMM yyyy HH:mm:ss";
myCulture.DateTimeFormat.longDatePattern = "dddd, d. MMMM yyyy";
myCulture.DateTimeFormat.longTimePattern = "HH:mm:ss";
myCulture.DateTimeFormat.monthDayPattern = "dd MMMM";
myCulture.DateTimeFormat.monthNames = ["Januar", "Februar", "M\xe4rz", "April", "Mai", "Juni", "Juli", "August", "September", "Oktober", "November", "Dezember", ""];
myCulture.DateTimeFormat.monthGenitiveNames = ["Januar", "Februar", "M\xe4rz", "April", "Mai", "Juni", "Juli", "August", "September", "Oktober", "November", "Dezember", ""];
myCulture.DateTimeFormat.shortDatePattern = "dd.MM.yyyy";
myCulture.DateTimeFormat.shortTimePattern = "HH:mm";
myCulture.DateTimeFormat.yearMonthPattern = "MMMM yyyy";
myCulture.DateTimeFormat.defaultDatePattern = "MM/dd/yyyy HH:mm:ss";
//add one culture
GC.Spread.Common.CultureManager.addCultureInfo("de-DE", myCulture);
//switch to "de-DE" culture
GC.Spread.Common.CultureManager.culture("de-DE");
var d = new Date();
//With culture
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate() + 1)));
activeSheet.getCell(1, 0).formatter("mmm");
var dvalue = 12345.6789;
activeSheet.setColumnWidth(0, 200);
activeSheet.setColumnWidth(1, 200);
activeSheet.setColumnWidth(2, 200);
activeSheet.setValue(0, 0, dvalue);
activeSheet.getCell(0, 0).formatter("###,###.00");
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate() + 1)));
//With culture
activeSheet.getCell(3, 0).formatter("yyyy/mmm/dddd");
activeSheet.setValue(3, 0, new Date());
```

___

### <a id="localnumberformat" name="localnumberformat"></a> LocalNumberFormat

• **LocalNumberFormat**: [`ILocalNumberFormat`](../interfaces/GC.Spread.Common.ILocalNumberFormat.md)

表示本地数字格式构建。它是一个键为数字、值为格式字符串的映射。

**`example`**
```
//this is an example for LocalNumberFormat.
var cultureInfo = new GC.Spread.Common.CultureInfo().
cultureInfo.LocalNumberFormat = {
 14:"yyyy-mm-dd",
 15:"yyyy/mm/dd"
}
```

___

### <a id="numberformat" name="numberformat"></a> NumberFormat

• **NumberFormat**: [`INumberFormat`](../interfaces/GC.Spread.Common.INumberFormat.md)

表示所有数字格式字段。

**`example`**
```
// This example creates a custom culture.
var myCulture = new GC.Spread.Common.CultureInfo();
myCulture.NumberFormat.currencySymbol = "\u20ac"
myCulture.NumberFormat.numberDecimalSeparator = ",";
myCulture.NumberFormat.numberGroupSeparator = ".";
myCulture.NumberFormat.arrayGroupSeparator = ";";
myCulture.NumberFormat.arrayListSeparator = "\\";
myCulture.NumberFormat.dbNumber = {
   1: {letters: ['\u5146', '\u5343', '\u767e', '\u5341', '\u4ebf', '\u5343', '\u767e', '\u5341', '\u4e07', '\u5343', '\u767e', '\u5341', ''], // \u5146\u5343\u767e\u5341\u4ebf\u5343\u767e\u5341\u4e07\u5343\u767e\u5341
       numbers: ['\u25cb', '\u4e00', '\u4e8c', '\u4e09', '\u56db', '\u4e94', '\u516d', '\u4e03', '\u516b', '\u4e5d'] }, // \u25cb\u4e00\u4e8c\u4e09\u56db\u4e94\u516d\u4e03\u516b\u4e5d
   2: {letters: ['\u5146', '\u4edf', '\u4f70', '\u62fe', '\u4ebf', '\u4edf', '\u4f70', '\u62fe', '\u4e07', '\u4edf', '\u4f70', '\u62fe', ''], // \u5146\u4edf\u4f70\u62fe\u4ebf\u4edf\u4f70\u62fe\u4e07\u4edf\u4f70\u62fe
       numbers: ['\u96f6', '\u58f9', '\u8d30', '\u53c1', '\u8086', '\u4f0d', '\u9646', '\u67d2', '\u634c', '\u7396']}, // \u96f6\u58f9\u8d30\u53c1\u8086\u4f0d\u9646\u67d2\u634c\u7396
   3: {letters: null,
       numbers: ['\uff10', '\uff11', '\uff12', '\uff13', '\uff14', '\uff15', '\uff16', '\uff17', '\uff18', '\uff19']} // \uff10\uff11\uff12\uff13\uff14\uff15\uff16\uff17\uff18\uff19
};
myCulture.NumberFormat.listSeparator = ";";
myCulture.DateTimeFormat.amDesignator = "";
myCulture.DateTimeFormat.pmDesignator = "";
myCulture.DateTimeFormat.abbreviatedMonthNames = ["Jan", "Feb", "Mrz", "Apr", "Mai", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dez", ""];
myCulture.DateTimeFormat.abbreviatedDayNames = ["So", "Mo", "Di", "Mi", "Do", "Fr", "Sa"];
myCulture.DateTimeFormat.abbreviatedMonthGenitiveNames = ["Jan", "Feb", "Mrz", "Apr", "Mai", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dez", ""];
myCulture.DateTimeFormat.dayNames = ["Sonntag", "Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag"];
myCulture.DateTimeFormat.fullDateTimePattern = "dddd, d. MMMM yyyy HH:mm:ss";
myCulture.DateTimeFormat.longDatePattern = "dddd, d. MMMM yyyy";
myCulture.DateTimeFormat.longTimePattern = "HH:mm:ss";
myCulture.DateTimeFormat.monthDayPattern = "dd MMMM";
myCulture.DateTimeFormat.monthNames = ["Januar", "Februar", "M\xe4rz", "April", "Mai", "Juni", "Juli", "August", "September", "Oktober", "November", "Dezember", ""];
myCulture.DateTimeFormat.monthGenitiveNames = ["Januar", "Februar", "M\xe4rz", "April", "Mai", "Juni", "Juli", "August", "September", "Oktober", "November", "Dezember", ""];
myCulture.DateTimeFormat.shortDatePattern = "dd.MM.yyyy";
myCulture.DateTimeFormat.shortTimePattern = "HH:mm";
myCulture.DateTimeFormat.yearMonthPattern = "MMMM yyyy";
//add one culture
GC.Spread.Common.CultureManager.addCultureInfo("de-DE", myCulture);
//switch to "de-DE" culture
GC.Spread.Common.CultureManager.culture("de-DE");
var d = new Date();
//With culture
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate() + 1)));
activeSheet.getCell(1, 0).formatter("mmm");
var dvalue = 12345.6789;
activeSheet.setColumnWidth(0, 200);
activeSheet.setColumnWidth(1, 200);
activeSheet.setColumnWidth(2, 200);
activeSheet.setValue(0, 0, dvalue);
activeSheet.getCell(0, 0).formatter("###,###.00");
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate() + 1)));
//With culture
activeSheet.getCell(3, 0).formatter("yyyy/mmm/dddd");
activeSheet.setValue(3, 0, new Date());
```

___

### <a id="textformat" name="textformat"></a> TextFormat

• **TextFormat**: [`ITextFormat`](../interfaces/GC.Spread.Common.ITextFormat.md)

表示文本格式字段。

**`example`**
```
// This example modify culture line breaking strategy.
var myCulture = GC.Spread.Common.CultureManager.getCultureInfo();
myCulture.TextFormat.lineBreakingChar = [" ", "+"]; // can line breaking when "+"
myCulture.TextFormat.lineBreakingForbidStart = ["\u300b"]; // the \u300bwon't be start of the breaking line
myCulture.TextFormat.lineBreakingForbidEnd = ["\u300a"]; // the \u300a won't be end of the breaking line
activeSheet.setValue(0, 0, "1. 1+2+3+4+5+6+7");
activeSheet.getCell(0, 0).wordWrap(true);  // the "1. " won't be in a single line
activeSheet.setValue(1, 0, "\u300aabc\u300b\u300adef\u300b\u300aghk\u300b");
activeSheet.getCell(1, 0).wordWrap(true);  // the\u300a \u300bwill looks better
```

___

### <a id="displayname" name="displayname"></a> displayName

• **displayName**: `string`

在格式对话框的位置下拉列表或符号下拉列表中显示的名称。

**`example`**
```
//This example set the displayName of CultureInfo:
var culture = new GC.Spread.Common.CultureInfo();
culture.displayName = "English(U.S.)"
```

___

### <a id="equalcharacters" name="equalcharacters"></a> equalCharacters

• **equalCharacters**: `string`[]

定义在计算中哪些字符被视为特殊相等的列表。

**`example`**
```
//This example sets the EqualCharacters of some characters:
var culture = new GC.Spread.Common.CultureInfo();
culture.equalCharacters = ["\u3002.", "\uff0c,", "\u24601\u4e00\u58f9"];
sheet.setFormula(0, 0, '"1.hello"="\u4e00\u3002Hello"'); // formula result will be TRUE after set culture.
```

___

### <a id="fontscriptcode" name="fontscriptcode"></a> fontScriptCode

• `Optional` **fontScriptCode**: `string`

主题用于查找字体的字体脚本代码。

**`example`**
```
//This example set the fontScriptCode of CultureInfo:
var culture = new GC.Spread.Common.CultureInfo();
culture.fontScriptCode = "Hans";
```

___

### <a id="id" name="id"></a> id

• **id**: `number`

可用于在数字格式中指定CultureInfo的ID。

**`example`**
```
//This example adds a new CultureInfo and affects the number format.
let culture = new GC.Spread.Common.CultureInfo();
culture.id = 0x407;
culture.NumberFormat.numberDecimalSeparator = ",";
culture.NumberFormat.numberGroupSeparator = ".";
culture.NumberFormat.listSeparator = "";
culture.name = function () { return "de-DE"; };
GC.Spread.Common.CultureManager.addCultureInfo(culture.name(), culture);
let formatter = new GC.Spread.Formatter.GeneralFormatter("[$-407]0,000.000");
let result = formatter.format(100000); //result: '100.000,000'
```

___

### <a id="predefinedformats" name="predefinedformats"></a> predefinedFormats

• **predefinedFormats**: [`IPredefinedFormats`](../interfaces/GC.Spread.Common.IPredefinedFormats.md)

predefinedFormats是一个描述格式对话框中部分数字格式的对象。
打开格式对话框时，设计器会读取所有CultureInfos中的predefinedFormats以显示与文化相关的格式。

**`example`**
```
//This is an example for predefinedFormats:
var culture = new GC.Spread.Common.CultureInfo()
culture.predefinedFormats = {
    Accounting: '_($* #,##0._);_($* (#,##0.);_($* "-"._);_(@_)',
    Currency: [
        "[$$-409]#,##0.",
        "[$$-409]#,##0.;[Red][$$-409]#,##0.",
        "[$$-409]#,##0._);([$$-409]#,##0.)",
        "[$$-409]#,##0._);[Red]([$$-409]#,##0.)"
    ],
    Date: [
        "m/d/yyyy",
        "[$-409]dddd, mmmm dd, yyyy",
        "m/d;@",
        "m/d/yy;@",
        "mm/dd/yy;@",
        "[$-409]d-mmm;@",
        "[$-409]d-mmm-yy;@",
        "[$-409]mmm-yy;@",
        "[$-409]mmmm-yy;@",
        "[$-409]mmmm d, yyyy;@",
        "[$-409]m/d/yy h:mm AM/PM;@",
        "m/d/yy h:mm;@",
        "[$-409]mmmmm;@",
        "[$-409]mmmmm-yy;@",
        "m/d/yyyy;@",
        "[$-409]d-mmm-yyyy;@",
    ],
    Time: [
        "[$-409]h:mm:ss AM/PM",
        "h:mm;@",
        "[$-409]h:mm AM/PM;@",
        "h:mm:ss;@",
        "[$-409]h:mm:ss AM/PM;@",
        "mm:ss.0;@",
        "[h]:mm:ss;@",
        "[$-409]m/d/yy h:mm AM/PM;@",
        "m/d/yy h:mm;@"
    ],
    Special: {
        "Zip Code": "00000",
        "Zip Code + 4": "00000-0000",
        "Phone Number": "[<=9999999]###-####;(###) ###-####",
        "Social Security Number": "000-00-0000"
    }
};
```

## Methods

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取CultureInfo的名称，如'de-DE'。

**`example`**
```
//This example adds and gets a new CultureInfo
let cultureInfo = new GC.Spread.Common.CultureInfo();
cultureInfo.id = 0x407;
cultureInfo.NumberFormat.numberDecimalSeparator = ",";
cultureInfo.NumberFormat.numberGroupSeparator = ".";
cultureInfo.NumberFormat.listSeparator = "";
cultureInfo.name = function () { return "de-DE"; };
GC.Spread.Common.CultureManager.addCultureInfo(cultureInfo.name(), cultureInfo);
console.log(cultureInfo === GC.Spread.Common.CultureManager.getCultureInfo("de-DE"));//output: true
```

#### Returns

`string`

CultureInfo的名称
