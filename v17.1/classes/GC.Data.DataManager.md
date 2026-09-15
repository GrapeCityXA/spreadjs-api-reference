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

数据管理器

**`代码示例`**
```
// 创建数据管理器
var dataManager = new GC.Data.DataManager();
```

## Properties

### <a id="relationships" name="relationships"></a> relationships

• **relationships**: [`IRelationship`](../interfaces/GC.Data.IRelationship.md)[]

关系数组每个关系包括以下字段,

**`property`** {GC.Data.Table} sourceTable - 源表

**`property`** {string} sourceFieldName - 源表的字段名

**`property`** {string} sourceRelationshipName - 可以在源表中使用的关系名称

**`property`** {GC.Data.Table} targetTable - 目标表

**`property`** {string} targetFieldName - 目标表的字段名

**`property`** {string} targetRelationshipName - 可在目标表中使用的关系名称

___

### <a id="tables" name="tables"></a> tables

• **tables**: [`ITables`](../interfaces/GC.Data.ITables.md)

表集合它的键是表名，值是GC.Data.Table 实例

## Methods

### <a id="addrelationship" name="addrelationship"></a> addRelationship

▸ **addRelationship**(`sourceTable`, `sourceFieldName`, `sourceRelationshipName`, `targetTable`, `targetFieldName`, `targetRelationshipName`): [`IRelationship`](../interfaces/GC.Data.IRelationship.md)

将关系添加到数据管理器中

**`代码示例`**
```
// 添加产品表和类别表之间的关系
dataManager.addRelationship(productTable, "categoryId", "categories", categoriesTable, "id", "products");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceTable` | [`Table`](GC.Data.Table.md) | 源表，其中外键是目标表的主键 |
| `sourceFieldName` | `string` | 源字段名称 |
| `sourceRelationshipName` | `string` | 关系名称 |
| `targetTable` | [`Table`](GC.Data.Table.md) | 目标表，其主键是源表的外键 |
| `targetFieldName` | `string` | 目标字段名 |
| `targetRelationshipName` | `string` | 目标关系名称 |

#### Returns

[`IRelationship`](../interfaces/GC.Data.IRelationship.md)

返回关系

___

### <a id="addtable" name="addtable"></a> addTable

▸ **addTable**(`name`, `dataSourceOption`): [`Table`](GC.Data.Table.md)

将表添加到数据管理器中

**`代码示例`**
```
// 添加示例表读取数据
var tableName = "products";
var dataSourceOption = {
     remote: {
        read: {
            url: "https://demodata.grapecity.com/northwind/api/v1/orders"
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
| `name` | `string` | 表格名称 |
| `dataSourceOption` | [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption) | 用于创建表的数据源选项 |

#### Returns

[`Table`](GC.Data.Table.md)

Returns the table.

___

### <a id="removerelationship" name="removerelationship"></a> removeRelationship

▸ **removeRelationship**(`name`): `void`

按源关系名称从数据管理器中删除关系

**`代码示例`**
```
// 按源关系名称从数据管理器中删除关系
dataManager.removeRelationship("categories");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 关系名称 |

#### Returns

`void`

___

### <a id="removetable" name="removetable"></a> removeTable

▸ **removeTable**(`name`): `void`

从数据管理器中删除表

**`代码示例`**
```
// 按表名从数据管理器中删除表
dataManager.removeTable("products");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表格名称 |

#### Returns

`void`
