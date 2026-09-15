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
- [id](GC.Spread.Common.CultureInfo.md#id)
- [predefinedFormats](GC.Spread.Common.CultureInfo.md#predefinedformats)

### Methods

- [name](GC.Spread.Common.CultureInfo.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CultureInfo**()

自定义本地化的类成员变量可以被覆盖

## Properties

### <a id="datetimeformat" name="datetimeformat"></a> DateTimeFormat

• **DateTimeFormat**: [`IDateTimeFormat`](../interfaces/GC.Spread.Common.IDateTimeFormat.md)

日期时间格式字段

**`property`** {string[]} abbreviatedDayNames - "ddd"的日期格式化

**`property`** {string[]} abbreviatedMonthGenitiveNames - "MMM"的月份格式化

**`property`** {string[]} abbreviatedMonthNames - "MMM"的月份格式化

**`property`** {string} amDesignator - AM表示器

**`property`** {string[]} dayNames - "dddd"的日期格式化

**`property`** {string} fullDateTimePattern - "F"的标准日期格式化

**`property`** {string} longDatePattern - "D"的标准日期格式化

**`property`** {string} longTimePattern - Specifies the standard date formatter for "T" and "U".

**`property`** {string} monthDayPattern - Specifies the standard date formatter for "M" and "m".

**`property`** {string[]} monthGenitiveNames - "MMMM"的格式化

**`property`** {string[]} monthNames - Specifies the formatter for "M" or "MM".

**`property`** {string} pmDesignator - PM表示器

**`property`** {string} shortDatePattern - "d"的标准日期格式化

**`property`** {string} shortTimePattern - "t"的标准日期格式化

**`property`** {string} yearMonthPattern - Specifies the standard date formatter for "y" and "Y".

**`代码示例`**
```
// 本示例创建了自定义本地化
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
//添加一个本地化信息
GC.Spread.Common.CultureManager.addCultureInfo("de-DE", myCulture);
//switch to "de-DE" culture
GC.Spread.Common.CultureManager.culture("de-DE");
var d = new Date();
//本地化
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate() + 1)));
activeSheet.getCell(1, 0).formatter("mmm");
var dvalue = 12345.6789;
activeSheet.setColumnWidth(0, 200);
activeSheet.setColumnWidth(1, 200);
activeSheet.setColumnWidth(2, 200);
activeSheet.setValue(0, 0, dvalue);
activeSheet.getCell(0, 0).formatter("###,###.00");
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate() + 1)));
//本地化
activeSheet.getCell(3, 0).formatter("yyyy/mmm/dddd");
activeSheet.setValue(3, 0, new Date());
```

___

### <a id="textformat" name="textformat"></a> TextFormat

• **TextFormat**: [`ITextFormat`](../interfaces/GC.Spread.Common.ITextFormat.md)

文本格式化字段

**`property`** {string[]} lineBreakingChar - 指定换行符，默认为 [" ", "-"].

**`property`** {string[]} lineBreakingForbidStart - 指定不允许出现在换行符开头的字符。

**`property`** {string[]} lineBreakingForbidEnd - 指定不允许出现在换行符结尾的字符。

**`property`** {GC.Spread.Common.ILineBreakingStrategy} lineBreakingStrategy - 指定单词拆分的函数。

**`example`**
```
// 一个修改本地化换行策略的例子
var myCulture = GC.Spread.Common.CultureManager.getCultureInfo();
myCulture.TextFormat.lineBreakingChar = [" ", "+"]; // 修改换行符为"+"
myCulture.TextFormat.lineBreakingForbidStart = ["\u300b"]; // 换行不会在"》"开始
myCulture.TextFormat.lineBreakingForbidEnd = ["\u300a"]; // 换行不会在"《"结束
activeSheet.setValue(0, 0, "1. 1+2+3+4+5+6+7");
activeSheet.getCell(0, 0).wordWrap(true);  // "1. "不会单独成行。
activeSheet.setValue(1, 0, "\u300aabc\u300b\u300adef\u300b\u300aghk\u300b"); // 值为"《abc》《def》《ghk》"
activeSheet.getCell(1, 0).wordWrap(true); 
```

___

### <a id="localnumberformat" name="localnumberformat"></a> LocalNumberFormat

• **LocalNumberFormat**: [`ILocalNumberFormat`](../interfaces/GC.Spread.Common.ILocalNumberFormat.md)

构建本地数字格式。它是一个映射,键是数字,值是格式字符串

**`property`** {string} key - 此属性的键是数字,此属性的值是格式字符串
//示例
var cultureInfo = new GC.Spread.Common.CultureInfo().
cultureInfo.LocalNumberFormat = {
 14:"yyyy-mm-dd",
 15:"yyyy/mm/dd"
}

___

### <a id="numberformat" name="numberformat"></a> NumberFormat

• **NumberFormat**: [`INumberFormat`](../interfaces/GC.Spread.Common.INumberFormat.md)

所有的数字格式字段

**`property`** {string} currencyDecimalSeparator - 货币小数点

**`property`** {string} currencyGroupSeparator - 货币千位分隔符

**`property`** {string} currencySymbol - 示货币符号

**`property`** {string} numberDecimalSeparator - 小数点

**`property`** {string} numberGroupSeparator - 千位分隔符

**`property`** {string} listSeparator - 公式中函数参数的分隔符

**`property`** {string} arrayListSeparator - 公式中数组常量的一行中的常量的分隔符

**`property`** {string} arrayGroupSeparator - 公式中数组常量的数组行的分隔符

**`property`** {object} dbNumber - 指定DBNumber字符
dbNumber对象的结构如下:
 {
    1: {letters: ['\u5146', '\u5343', '\u767e', '\u5341', '\u4ebf', '\u5343', '\u767e', '\u5341', '\u4e07', '\u5343', '\u767e', '\u5341', ''], // \u5146\u5343\u767e\u5341\u4ebf\u5343\u767e\u5341\u4e07\u5343\u767e\u5341
        numbers: ['\u25cb', '\u4e00', '\u4e8c', '\u4e09', '\u56db', '\u4e94', '\u516d', '\u4e03', '\u516b', '\u4e5d'] }, // \u25cb\u4e00\u4e8c\u4e09\u56db\u4e94\u516d\u4e03\u516b\u4e5d
    2: {letters: ['\u5146', '\u4edf', '\u4f70', '\u62fe', '\u4ebf', '\u4edf', '\u4f70', '\u62fe', '\u4e07', '\u4edf', '\u4f70', '\u62fe', ''], // \u5146\u4edf\u4f70\u62fe\u4ebf\u4edf\u4f70\u62fe\u4e07\u4edf\u4f70\u62fe
        numbers: ['\u96f6', '\u58f9', '\u8d30', '\u53c1', '\u8086', '\u4f0d', '\u9646', '\u67d2', '\u634c', '\u7396']}, // \u96f6\u58f9\u8d30\u53c1\u8086\u4f0d\u9646\u67d2\u634c\u7396
    3: {letters: null,
        numbers: ['\uff10', '\uff11', '\uff12', '\uff13', '\uff14', '\uff15', '\uff16', '\uff17', '\uff18', '\uff19']} // \uff10\uff11\uff12\uff13\uff14\uff15\uff16\uff17\uff18\uff19
};

**`代码示例`**
```
// 本示例创建了自定义本地化
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
//添加一个本地化信息
GC.Spread.Common.CultureManager.addCultureInfo("de-DE", myCulture);
//switch to "de-DE" culture
GC.Spread.Common.CultureManager.culture("de-DE");
var d = new Date();
//本地化
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate() + 1)));
activeSheet.getCell(1, 0).formatter("mmm");
var dvalue = 12345.6789;
activeSheet.setColumnWidth(0, 200);
activeSheet.setColumnWidth(1, 200);
activeSheet.setColumnWidth(2, 200);
activeSheet.setValue(0, 0, dvalue);
activeSheet.getCell(0, 0).formatter("###,###.00");
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate() + 1)));
//本地化
activeSheet.getCell(3, 0).formatter("yyyy/mmm/dddd");
activeSheet.setValue(3, 0, new Date());
```

___

### <a id="displayname" name="displayname"></a> displayName

• **displayName**: `string`

___

### <a id="id" name="id"></a> id

• **id**: `number`

id可以用来指定数字格式的CultureInfo

___

### <a id="predefinedformats" name="predefinedformats"></a> predefinedFormats

• **predefinedFormats**: [`IPredefinedFormats`](../interfaces/GC.Spread.Common.IPredefinedFormats.md)

## Methods

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取CultureInfo的名称,例如 "de-DE"

#### Returns

`string`

**`代码示例`**
```
The name of the CultureInfo
//本示例添加和获取了一个新的CultureInfo
let cultureInfo = new GC.Spread.Common.CultureInfo();
cultureInfo.id = 0x407;
cultureInfo.NumberFormat.numberDecimalSeparator = ",";
cultureInfo.NumberFormat.numberGroupSeparator = ".";
cultureInfo.NumberFormat.listSeparator = "";
cultureInfo.name = function () { return "de-DE"; };
GC.Spread.Common.CultureManager.addCultureInfo(cultureInfo.name(), cultureInfo);
console.log(cultureInfo === GC.Spread.Common.CultureManager.getCultureInfo("de-DE"));//输出: true
___