# Class: DataManager

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).DataManager

## Table of contents

### Constructors

- [constructor](GC.Data.DataManager.md#constructor)

### Properties

- [relationships](GC.Data.DataManager.md#relationships)
- [tables](GC.Data.DataManager.md#tables)

### Methods

- [addRelationship](GC.Data.DataManager.md#addrelationship)
- [addTable](GC.Data.DataManager.md#addtable)
- [removeRelationship](GC.Data.DataManager.md#removerelationship)
- [removeTable](GC.Data.DataManager.md#removetable)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataManager**()

表示数据管理器。

**`example`**
```javascript
// 创建一个数据管理器
var dataManager = new GC.Data.DataManager();
```

## Properties

### <a id="relationships" name="relationships"></a> relationships

• **relationships**: [`IRelationship`](../interfaces/GC.Data.IRelationship.md)[]

表示关系数组。每个关系包含以下字段：

**`property`** {GC.Data.Table} sourceTable - 源表。

**`property`** {string} sourceFieldName - 源表的字段名。

**`property`** {string} sourceRelationshipName - 可在源表中使用的关系名称。

**`property`** {GC.Data.Table} targetTable - 目标表。

**`property`** {string} targetFieldName - 目标表的字段名。

**`property`** {string} targetRelationshipName - 可在目标表中使用的关系名称。

___

### <a id="tables" name="tables"></a> tables

• **tables**: [`ITables`](../interfaces/GC.Data.ITables.md)

表示表集合。其键是表名，值是GC.Data.Table实例。

## Methods

### <a id="addrelationship" name="addrelationship"></a> addRelationship

▸ **addRelationship**(`sourceTable`, `sourceFieldName`, `sourceRelationshipName`, `targetTable`, `targetFieldName`, `targetRelationshipName`): [`IRelationship`](../interfaces/GC.Data.IRelationship.md)

向数据管理器添加一个关系。

**`example`**
```javascript
// 在产品表和类别表之间添加关系
dataManager.addRelationship(productTable, "categoryId", "categories", categoriesTable, "id", "products");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceTable` | [`Table`](GC.Data.Table.md) | 源表，其外键是目标表的主键。 |
| `sourceFieldName` | `string` | 源字段名。 |
| `sourceRelationshipName` | `string` | 源关系名称。 |
| `targetTable` | [`Table`](GC.Data.Table.md) | 目标表，其主键是源表的外键。 |
| `targetFieldName` | `string` | 目标字段名。 |
| `targetRelationshipName` | `string` | 目标关系名称。 |

#### Returns

[`IRelationship`](../interfaces/GC.Data.IRelationship.md)

返回该关系。

___

### <a id="addtable" name="addtable"></a> addTable

▸ **addTable**(`name`, `dataSourceOption`): [`Table`](GC.Data.Table.md)

向数据管理器添加一个表。

**`example`**
```javascript
// 添加一个示例表以读取数据
var tableName = "products";
var dataSourceOption = {
     remote: {
        read: {
            url: "https://demodata.grapecity.com/northwind/api/v1/Orders"
        }
    },
    schema: {
        columns: {
            orderId: {dataName: "id"},
            orderDate: {dataType: "date", dataPattern: "yyyy-MM-dd hh:mm:ss.000"},
            requiredDate: {dataType: "date"},
            shippedDate: {dataType: "date"},
            shipVia: {dataMap: {1: "Speedy Express", 2: "United Package", 3: "Federal Shipping"}}
        }
    }
};
var dataManager = new GC.Data.DataManager();
var productTable = dataManager.addTable(tableName, dataSourceOption);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表名。 |
| `dataSourceOption` | [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption) | 用于创建表的数据源选项，包含以下属性。 |

#### Returns

[`Table`](GC.Data.Table.md)

返回该表。

___

### <a id="removerelationship" name="removerelationship"></a> removeRelationship

▸ **removeRelationship**(`name`): `void`

通过源关系名称从数据管理器中移除一个关系。

**`example`**
```javascript
// 通过源关系名称从数据管理器中移除一个关系
dataManager.removeRelationship("categories");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 源关系名称。 |

#### Returns

`void`

___

### <a id="removetable" name="removetable"></a> removeTable

▸ **removeTable**(`name`): `void`

从数据管理器中移除一个表。

**`example`**
```javascript
// 通过表名从数据管理器中移除一个表
dataManager.removeTable("products");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表名。 |

#### Returns

`void`
