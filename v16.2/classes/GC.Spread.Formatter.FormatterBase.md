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

## Methods

### <a id="format" name="format"></a> format

▸ **format**(`obj`): `string`

将指定的对象格式化为带有条件颜色的字符串这个函数应该重写

**`代码示例`**
```
//本示例创建了一个自定义格式化程序
var customFormatterTest = {};
customFormatterTest.prototype = GC.Spread.Formatter.FormatterBase;
customFormatterTest.format = function (obj, data) {
    data.conditionalForeColor = "blue";
    return "My format result : " + obj.toString();
};
customFormatterTest.parse = function (str) {
    if (!str) {
        return "";
    }
    return str;
}
activeSheet.getCell(1, 0).formatter(customFormatterTest);
activeSheet.getCell(1, 0).value("Test");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object` | 要格式化单元格数据的对象 |

#### Returns

`string`

格式化的字符串

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态

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

**`代码示例`**
```
//本示例创建了一个自定义格式化程序
var customFormatterTest = {};
customFormatterTest.prototype = GC.Spread.Formatter.FormatterBase;
customFormatterTest.format = function (obj, conditionalForeColor) {
    conditionalForeColor.value = "blue";
    return "My format result : " + obj.toString();
};
customFormatterTest.parse = function (str) {
    if (!str) {
        return "";
    }
    return str;
}
activeSheet.getCell(1, 0).formatter(customFormatterTest);
activeSheet.getCell(1, 0).value("Test")
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

#### Returns

`Object`

解析对象

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串

#### Returns

`Object`

自定义格式化数据
