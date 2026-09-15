# Class: FloatingObjectCollection

[Sheets](../modules/GC.Spread.Sheets.md).[FloatingObjects](../modules/GC.Spread.Sheets.FloatingObjects.md).FloatingObjectCollection

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#add)
- [all](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#all)
- [clear](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#clear)
- [get](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#get)
- [remove](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#remove)
- [zIndex](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FloatingObjectCollection**(`sheet?`, `typeName?`)

表示一个浮动对象管理器，用于管理工作表中的所有浮动对象。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |
| `typeName?` | `string` | 类型名称。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`floatingObjectOrName`, `src?`, `x?`, `y?`, `width?`, `height?`): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

向工作表中添加浮动对象。
参数有两种模式：
如果只有1个参数，该参数是floatingObject，类型为GC.Spread.Sheets.FloatingObjects.FloatingObject。
如果有6个参数，参数分别是name、src、x、y、width和height。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
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
| `floatingObjectOrName` | `string` \| [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md) | 要添加到工作表的浮动对象，或要添加到工作表的图片名称。 |
| `src?` | `string` | 图片的图像源。 |
| `x?` | `number` | 图片的x位置。 |
| `y?` | `number` | 图片的y位置。 |
| `width?` | `number` | 图片的宽度。 |
| `height?` | `number` | 图片的高度。 |

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

已添加到工作表的浮动对象。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)[]

获取工作表中的所有浮动对象。

**`example`**
```javascript
activeSheet.pictures.add("p1", "pics/download.jpg", 1, 6, 400, 400);
activeSheet.pictures.add("p2", "pics/download.jpg", 500, 150, 200, 300);
var pictures = activeSheet.pictures.all();
for (var i = 0; i &lt; pictures.length; i++) {
    alert("Path of picture " + i + " is:  " + pictures[i].src())
}
```

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)[]

工作表中所有浮动对象的集合。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

移除工作表中的所有浮动对象。

**`example`**
```javascript
var f1 = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 64, 30);
f1.content(createButton('button 1', '64px', '30px'));
activeSheet.floatingObjects.add(f1);

var f2 = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f2', 100, 10, 64, 30);
f2.content(createButton('button 2', '64px', '30px'));
activeSheet.floatingObjects.add(f2);

console.log(activeSheet.floatingObjects.all().length); // 结果是 2
activeSheet.floatingObjects.clear(); // 移除所有浮动对象
console.log(activeSheet.floatingObjects.all().length); // 结果是 0

function createButton (text, width, height) {
    var btn = document.createElement('button');
    btn.style.width = width;
    btn.style.height = height;
    btn.innerText = text;
    return btn;
}
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

通过指定名称获取工作表中的浮动对象。

**`example`**
```javascript
activeSheet.pictures.add("f2","tsoutline.png",100,60,200,100);
//button
$("#button1").click(function () {
 var pic = activeSheet.pictures.get("f2");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 浮动对象的名称。 |

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

工作表中具有指定名称的浮动对象。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

通过指定名称从工作表中移除浮动对象。

**`example`**
```javascript
activeSheet.pictures.add("f2","tsoutline.png",100,60,200,100);
//button
$("#button1").click(function () {
     activeSheet.resumePaint();
     activeSheet.pictures.remove("f2");
     activeSheet.repaint();
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 浮动对象的名称。 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`name`, `zIndex?`): `any`

获取或设置浮动对象的z-index。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 20, 20, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button1";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
var customFloatingObject1 = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f2", 5, 5, 30, 64);
var btn1 = document.createElement('button');
btn1.style.width = "60px";
btn1.style.height = "30px";
btn1.innerText = "button2";
customFloatingObject1.content(btn1);
activeSheet.floatingObjects.add(customFloatingObject1);
activeSheet.floatingObjects.zIndex("f2", 897);
activeSheet.floatingObjects.zIndex("f1", 898);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 浮动对象的名称。 |
| `zIndex?` | `number` | 浮动对象的z-index。 |

#### Returns

`any`

如果参数'zIndex'为null或undefined，则返回具有指定名称的浮动对象的z-index。
