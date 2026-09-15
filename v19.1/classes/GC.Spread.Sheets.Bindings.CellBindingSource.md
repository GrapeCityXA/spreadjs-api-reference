# Class: CellBindingSource

[Sheets](../modules/GC.Spread.Sheets.md).[Bindings](../modules/GC.Spread.Sheets.Bindings.md).CellBindingSource

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Bindings.CellBindingSource.md#constructor)

### Methods

- [getSource](GC.Spread.Sheets.Bindings.CellBindingSource.md#getsource)
- [getValue](GC.Spread.Sheets.Bindings.CellBindingSource.md#getvalue)
- [setValue](GC.Spread.Sheets.Bindings.CellBindingSource.md#setvalue)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CellBindingSource**(`source`)

表示单元格绑定的数据源。

**`example`**
```javascript
var person = {name: "Wang feng", age: 25, address: {postcode: "710075"}};
var source = new GC.Spread.Sheets.Bindings.CellBindingSource(person);
activeSheet.setBindingPath(0, 0, "name");
activeSheet.setBindingPath(1, 1, "age");
activeSheet.setBindingPath(3, 3, "address.postcode");
activeSheet.setDataSource(source);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `Object` | 数据源。 |

## Methods

### <a id="getsource" name="getsource"></a> getSource

▸ **getSource**(): `Object`

获取单元格绑定的包装数据源。

**`example`**
```javascript
//此示例获取名称。
var person = { name: "Wang feng", age: 25, address: { postcode: "710075" } };
var source = new GC.Spread.Sheets.Bindings.CellBindingSource(person);
activeSheet.setBindingPath(0, 0, "name");
activeSheet.setBindingPath(1, 1, "age");
activeSheet.setBindingPath(3, 3, "address.postcode");
activeSheet.setDataSource(source);
alert(source.getSource().name);
```

#### Returns

`Object`

原始数据源。

___

### <a id="getvalue" name="getvalue"></a> getValue

▸ **getValue**(`path`): `Object`

通过绑定路径获取数据源的值。

**`example`**
```javascript
//此示例获取值。
var person = {name: "Wang feng", age: 25, address: {postcode: "710075"}};
var source = new GC.Spread.Sheets.Bindings.CellBindingSource(person);
activeSheet.setBindingPath(0, 0, "name");
activeSheet.setBindingPath(1, 1, "age");
activeSheet.setBindingPath(3, 3, "address.postcode");
activeSheet.setDataSource(source);
alert(source.getValue("name"));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 绑定路径。 |

#### Returns

`Object`

返回指定路径下绑定数据源的值。

___

### <a id="setvalue" name="setvalue"></a> setValue

▸ **setValue**(`path`, `value`): `void`

通过绑定路径设置数据源的值。

**`example`**
```javascript
//此示例设置名称值。
var person = {name: "Wang feng", age: 25, address: {postcode: "710075"}};
var source = new GC.Spread.Sheets.Bindings.CellBindingSource(person);
activeSheet.setBindingPath(0, 0, "name");
activeSheet.setBindingPath(1, 1, "age");
activeSheet.setBindingPath(3, 3, "address.postcode");
activeSheet.setDataSource(source);
source.setValue("name", "test");
activeSheet.resumePaint();
activeSheet.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 行索引。 |
| `value` | `Object` | 要设置的值。 |

#### Returns

`void`
