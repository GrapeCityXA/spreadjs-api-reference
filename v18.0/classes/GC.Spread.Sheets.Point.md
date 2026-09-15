# Class: Point

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Point

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Point.md#constructor)

### Methods

- [clone](GC.Spread.Sheets.Point.md#clone)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Point**(`x`, `y`)

二维空间中一个<i>x</i>和<i>y</i>的坐标对

**`代码示例`**
``` javascript
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
var point = new GC.Spread.Sheets.Point(10, 10);
customFloatingObject.position(point);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | <i>x</i>坐标 |
| `y` | `number` | <i>y</i>坐标 |

## Methods

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`Point`](GC.Spread.Sheets.Point.md)

从当前点克隆一个新的点

#### Returns

[`Point`](GC.Spread.Sheets.Point.md)

克隆的对象
