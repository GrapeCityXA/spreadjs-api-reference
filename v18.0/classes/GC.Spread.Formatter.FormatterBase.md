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

具有指定格式字符串的自定义格式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `format` | `string` | 格式化 |
| `cultureName` | `string` | 本地化名称 |

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

**`example`**
```
//This example creates a custom formatter.
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

将指定的对象格式化为带有条件颜色的字符串这个函数应该重写

**`代码示例`**
``` javascript
//This example creates a custom formatter.
function CustomFormatterTest() {
}
CustomFormatterTest.prototype = new GC.Spread.Formatter.FormatterBase();
CustomFormatterTest.prototype.format = function (obj, options) {
\xa0 \xa0 //if the obj is color string, exp: red, blue.the text will render with obj color.
\xa0 \xa0 if (obj) {
\xa0 \xa0 \xa0 \xa0 options.conditionalForeColor = obj.toString()
\xa0 \xa0 \xa0 \xa0 return "My format result : " + obj.toString();
\xa0 \xa0 }
\xa0 \xa0 return "";
};
CustomFormatterTest.prototype.parse = function (str) {
\xa0 \xa0 if (!str) {
\xa0 \xa0 \xa0 \xa0 return "";
\xa0 \xa0 }
\xa0 \xa0 return str;
}
var sheet = spread.getActiveSheet();
sheet.getCell(1, 0).formatter(new CustomFormatterTest());
sheet.getCell(1, 0).value("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object` | The object with cell data to format. |
| `options?` | `Object` | - |

#### Returns

`string`

格式化的字符串

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态

**`example`**
```
//This example creates a custom formatter.
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
| `settings` | `Object` | 来自反序列化的自定义格式化数据 |

#### Returns

`void`

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`str`): `Object`

解析指定的文本这个函数应被重写

**`example`**
```
//This example creates a custom formatter.
function CustomFormatterTest() {
}
CustomFormatterTest.prototype = new GC.Spread.Formatter.FormatterBase();
CustomFormatterTest.prototype.format = function (obj, options) {
\xa0 \xa0 //if the obj is color string, exp: red, blue.the text will render with obj color.
\xa0 \xa0 if (obj) {
\xa0 \xa0 \xa0 \xa0 options.conditionalForeColor = obj.toString()
\xa0 \xa0 \xa0 \xa0 return "My format result : " + obj.toString();
\xa0 \xa0 }
\xa0 \xa0 return "";
};
CustomFormatterTest.prototype.parse = function (str) {
\xa0 \xa0 if (!str) {
\xa0 \xa0 \xa0 \xa0 return "";
\xa0 \xa0 }
\xa0 \xa0 return str;
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

解析的对象

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串

**`example`**
```
//This example creates a custom formatter.
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

自定义格式化数据
