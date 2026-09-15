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

一个浮动对象元素管理器,用于管理表单中的所有浮动对象元素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 表单 |
| `typeName?` | `string` | 类型名称 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`floatingObjectOrName`, `src?`, `x?`, `y?`, `width?`, `height?`): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

将浮动对象元素添加到表
参数有2种模式
如果有1个参数,则该参数为floatObject,这是GC.Spread.Sheets.FloatingObjects.FloatingObject类型
如果有6个参数,则参数为name, src, x, y, width, 和 height

**`代码示例`**
```
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
| `floatingObjectOrName` | `string` \| [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md) | 将添加到表单的浮动对象,或将添加到表单的图片的名称 |
| `src?` | `string` | 图片的图像来源 |
| `x?` | `number` | 图片的x位置 |
| `y?` | `number` | 图片的y位置 |
| `width?` | `number` | 图片的宽度 |
| `height?` | `number` | 图片的高度 |

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

已添加到表的浮动对象元素

___

### <a id="all" name="all"></a> all

▸ **all**(): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)[]

获取表单表中的所有浮动对象元素

**`代码示例`**
```
activeSheet.pictures.add("p1", "pics/download.jpg", 1, 6, 400, 400);
activeSheet.pictures.add("p2", "pics/download.jpg", 500, 150, 200, 300);
var pictures = activeSheet.pictures.all();
for (var i = 0; i &lt; pictures.length; i++) {
    alert("Path of picture " + i + " is:  " + pictures[i].src())
}
```

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)[]

表单中所有浮动对象元素的集合

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

删除表单中的所有浮动对象元素

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

从表中通过指示名称获取一个浮动对象元素

**`代码示例`**
```
activeSheet.pictures.add("f2","tsoutline.png",100,60,200,100);
//button
$("#button1").click(function () {
 var pic = activeSheet.pictures.get("f2");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 浮动对象元素的名称 |

#### Returns

[`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

表单中带有指示名称的浮动对象元素

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

通过指示名称从表单中删除一个浮动对象元素

**`代码示例`**
```
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
| `name` | `string` | 浮动对象元素的名称 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`name`, `zIndex?`): `any`

获取或设置浮动对象元素的z-index

**`代码示例`**
```
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
| `name` | `string` | 浮动对象元素的名称 |
| `zIndex?` | `number` | 浮动对象元素的z-index |

#### Returns

`any`

如果参数'z-Index'为null或undefined,它将返回带有指示名称的浮动对象元素的z-index
