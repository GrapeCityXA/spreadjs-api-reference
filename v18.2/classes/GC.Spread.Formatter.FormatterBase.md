# Class: FormatterBase

[Spread](../modules/GC.Spread.md).[Formatter](../modules/GC.Spread.Formatter.md).FormatterBase

## Table of contents

### Constructors

- [constructor](GC.Spread.Formatter.FormatterBase.md#constructor)

### Properties

- [typeName](GC.Spread.Formatter.FormatterBase.md#typename)

### Methods

- [format](GC.Spread.Formatter.FormatterBase.md#format)
- [fromJSON](GC.Spread.Formatter.FormatterBase.md#fromjson)
- [parse](GC.Spread.Formatter.FormatterBase.md#parse)
- [toJSON](GC.Spread.Formatter.FormatterBase.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FormatterBase**(`format`, `cultureName`)

表示具有指定格式字符串的自定义格式化程序。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `format` | `string` | 格式字符串。 |
| `cultureName` | `string` | 区域性名称。 |

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

**`example`**
```
// 此示例创建一个自定义格式化程序。
function MyFormatter(format, cultureName) {
  GC.Spread.Formatter.FormatterBase.apply(this, arguments);
  this.typeName = "MyFormatter";
  this.formatter = format;
}
MyFormatter.prototype = new GC.Spread.Formatter.FormatterBase();
MyFormatter.prototype.format = function (obj, options) {
    if (typeof obj === "number") {
        var colors = this.formatter.split(";");
        if (obj >= 0) {
            options && options.conditionalForeColor = colors[0];
            return "PositiveOrZero: " + obj;
        } else {
            options && options.conditionalForeColor = colors[1];
            return "Negative: " + obj;
        }
    }
    return obj ? obj.toString() : "";
};
MyFormatter.prototype.parse = function (str) {
    var index = str.indexOf(": ");
    if (index >= 0) {
        return +str.substr(index + 2);
    } else {
        return +str;
    }
};
MyFormatter.prototype.toJSON = function () {
    return {
        typeName: this.typeName,
        formatter: this.formatter
    };
};
MyFormatter.prototype.fromJSON = function (settings) {
    if (settings) {
        this.formatter = settings.formatter;
    }
};
var formatter = new MyFormatter("red;green");
formatter.format(12345); // "PositiveOrZero: 12345"
formatter.parse("PositiveOrZero: 12345"); // 12345
```

## Methods

### <a id="format" name="format"></a> format

▸ **format**(`obj`, `options?`): `string`

使用条件颜色将指定对象格式化为字符串。此函数应被重写。

**`example`**
```
// 此示例创建一个自定义格式化程序。
function CustomFormatterTest() {
}
CustomFormatterTest.prototype = new GC.Spread.Formatter.FormatterBase();
CustomFormatterTest.prototype.format = function (obj, options) {
    // 如果 obj 是颜色字符串（如：red, blue），文本将使用该颜色渲染。
    if (obj) {
        options.conditionalForeColor = obj.toString()
        return "My format result : " + obj.toString();
    }
    return "";
};
CustomFormatterTest.prototype.parse = function (str) {
    if (!str) {
        return "";
    }
    return str;
}
var sheet = spread.getActiveSheet();
sheet.getCell(1, 0).formatter(new CustomFormatterTest());
sheet.getCell(1, 0).value("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object` | 要格式化的单元格数据对象。 |
| `options?` | `Object` | - |

#### Returns

`string`

格式化后的字符串。

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的 JSON 字符串加载对象状态。

**`example`**
```
// 此示例创建一个自定义格式化程序。
function MyFormatter(format, cultureName) {
  GC.Spread.Formatter.FormatterBase.apply(this, arguments);
  this.typeName = "MyFormatter";
  this.formatter = format;
}
MyFormatter.prototype = new GC.Spread.Formatter.FormatterBase();
MyFormatter.prototype.format = function (obj, options) {
    if (typeof obj === "number") {
        var colors = this.formatter.split(";");
        if (obj >= 0) {
            options && options.conditionalForeColor = colors[0];
            return "PositiveOrZero: " + obj;
        } else {
            options && options.conditionalForeColor = colors[1];
            return "Negative: " + obj;
        }
    }
    return obj ? obj.toString() : "";
};
MyFormatter.prototype.parse = function (str) {
    var index = str.indexOf(": ");
    if (index >= 0) {
        return +str.substr(index + 2);
    } else {
        return +str;
    }
};
MyFormatter.prototype.toJSON = function () {
    return {
        typeName: this.typeName,
        formatter: this.formatter
    };
};
MyFormatter.prototype.fromJSON = function (settings) {
    if (settings) {
        this.formatter = settings.formatter;
    }
};
var formatter = new MyFormatter("red;green");
formatter.format(12345); // "PositiveOrZero: 12345"
formatter.parse("PositiveOrZero: 12345"); // 12345
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `Object` | 反序列化得到的自定义格式化程序数据。 |

#### Returns

`void`

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`str`): `Object`

解析指定的文本。此函数应被重写。

**`example`**
```
// 此示例创建一个自定义格式化程序。
function CustomFormatterTest() {
}
CustomFormatterTest.prototype = new GC.Spread.Formatter.FormatterBase();
CustomFormatterTest.prototype.format = function (obj, options) {
    // 如果 obj 是颜色字符串（如：red, blue），文本将使用该颜色渲染。
    if (obj) {
        options.conditionalForeColor = obj.toString()
        return "My format result : " + obj.toString();
    }
    return "";
};
CustomFormatterTest.prototype.parse = function (str) {
    if (!str) {
        return "";
    }
    return str;
}
var sheet = spread.getActiveSheet();
sheet.getCell(1, 0).formatter(new CustomFormatterTest());
sheet.getCell(1, 0).value("red");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

#### Returns

`Object`

解析后的对象。

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为 JSON 字符串。

**`example`**
```
// 此示例创建一个自定义格式化程序。
function MyFormatter(format, cultureName) {
  GC.Spread.Formatter.FormatterBase.apply(this, arguments);
  this.typeName = "MyFormatter";
  this.formatter = format;
}
MyFormatter.prototype = new GC.Spread.Formatter.FormatterBase();
MyFormatter.prototype.format = function (obj, options) {
    if (typeof obj === "number") {
        var colors = this.formatter.split(";");
        if (obj >= 0) {
            options && options.conditionalForeColor = colors[0];
            return "PositiveOrZero: " + obj;
        } else {
            options && options.conditionalForeColor = colors[1];
            return "Negative: " + obj;
        }
    }
    return obj ? obj.toString() : "";
};
MyFormatter.prototype.parse = function (str) {
    var index = str.indexOf(": ");
    if (index >= 0) {
        return +str.substr(index + 2);
    } else {
        return +str;
    }
};
MyFormatter.prototype.toJSON = function () {
    return {
        typeName: this.typeName,
        formatter: this.formatter
    };
};
MyFormatter.prototype.fromJSON = function (settings) {
    if (settings) {
        this.formatter = settings.formatter;
    }
};
var formatter = new MyFormatter("red;green");
formatter.format(12345); // "PositiveOrZero: 12345"
formatter.parse("PositiveOrZero: 12345"); // 12345
```

#### Returns

`Object`

自定义格式化程序数据。
