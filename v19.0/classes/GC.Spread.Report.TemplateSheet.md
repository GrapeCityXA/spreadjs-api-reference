# Class: TemplateSheet

[Spread](../modules/GC.Spread.md).[Report](../modules/GC.Spread.Report.md).TemplateSheet

## Hierarchy

- [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

  ↳ **`TemplateSheet`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Report.TemplateSheet.md#constructor)

### Methods

- [getDataEntrySetting](GC.Spread.Report.TemplateSheet.md#getdataentrysetting)
- [getLayoutSetting](GC.Spread.Report.TemplateSheet.md#getlayoutsetting)
- [getPaginationSetting](GC.Spread.Report.TemplateSheet.md#getpaginationsetting)
- [getTemplateCell](GC.Spread.Report.TemplateSheet.md#gettemplatecell)
- [setDataEntrySetting](GC.Spread.Report.TemplateSheet.md#setdataentrysetting)
- [setLayoutSetting](GC.Spread.Report.TemplateSheet.md#setlayoutsetting)
- [setPaginationSetting](GC.Spread.Report.TemplateSheet.md#setpaginationsetting)
- [setTemplateCell](GC.Spread.Report.TemplateSheet.md#settemplatecell)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TemplateSheet**(`name`)

表示一个 TemplateSheet。

**`example`**
```
const spread = new GC.Spread.Sheets.Workbook('spread-host', { sheetCount: 0 });
const reportSheet = spread.addSheetTab(0, 'orders-report', GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = reportSheet.getTemplate();
templateSheet.setValue(0, 0, 'test');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 模板表的名称。 |

#### Overrides

[Worksheet](GC.Spread.Sheets.Worksheet.md).[constructor](GC.Spread.Sheets.Worksheet.md#constructor)

## Methods

### <a id="getdataentrysetting" name="getdataentrysetting"></a> getDataEntrySetting

▸ **getDataEntrySetting**(): [`DataEntrySetting`](../modules/GC.Spread.Report.md#dataentrysetting)

获取数据输入设置。

**`example`**
```
// 获取数据输入设置。
const dataEntrySetting = templateSheet.getDataEntrySetting();
```

#### Returns

[`DataEntrySetting`](../modules/GC.Spread.Report.md#dataentrysetting)

返回数据输入设置。

___

### <a id="getlayoutsetting" name="getlayoutsetting"></a> getLayoutSetting

▸ **getLayoutSetting**(): [`LayoutSetting`](../modules/GC.Spread.Report.md#layoutsetting)

获取布局设置。

**`example`**
```
// 获取布局设置。
const layoutSetting = templateSheet.getLayoutSetting();
```

#### Returns

[`LayoutSetting`](../modules/GC.Spread.Report.md#layoutsetting)

返回布局设置。

___

### <a id="getpaginationsetting" name="getpaginationsetting"></a> getPaginationSetting

▸ **getPaginationSetting**(): [`IPaginationSetting`](../interfaces/GC.Spread.Report.IPaginationSetting.md)

获取分页设置。

**`example`**
```
// 获取分页设置。
const paginationSetting = templateSheet.getPaginationSetting();
```

#### Returns

[`IPaginationSetting`](../interfaces/GC.Spread.Report.IPaginationSetting.md)

返回分页设置。

___

### <a id="gettemplatecell" name="gettemplatecell"></a> getTemplateCell

▸ **getTemplateCell**(`row`, `col`): [`TemplateCell`](../modules/GC.Spread.Report.md#templatecell)

获取模板单元格。

**`example`**
```
// 获取 A2 模板单元格的设置。
const templateCell = templateSheet.getTemplateCell(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`TemplateCell`](../modules/GC.Spread.Report.md#templatecell)

返回模板单元格。

___

### <a id="setdataentrysetting" name="setdataentrysetting"></a> setDataEntrySetting

▸ **setDataEntrySetting**(`dataEntrySetting`): `void`

设置数据输入设置。

**`example`**
```
// 添加 customers 表。
const customersTable = spread.dataManager().addTable('Customers', {
    remote: {
        read: { url: 'https://demodata.grapecity.com//northwind/api/v1/customers' },
        batch: (data) => {
            // 同步变更到服务端
            console.log('changes: ', data);
            return Promise.resolve(data.map((item) => ({ succeed: true })));
        },
    },
    batch: true,
});

// 为模板设置绑定
const columns = ['customerId', 'companyName', 'contactName', 'contactTitle', 'address', 'region', 'country', 'city', 'postalCode', 'phone', 'fax'];
columns.forEach((columnName, i) => {
    templateSheet.setValue(0, i, `${columnName[0].toUpperCase()}${columnName.substring(1)}`);
    templateSheet.setTemplateCell(1, i, {
        type: 'List',
        binding: `Customers[${columnName}]`,
    });
});

// 配置数据输入设置
const customerRule = {
    name: 'customers',
    tableName: 'Customers',
    fields: [
        { formula: 'A2', dbColumnName: 'customerId', isPrimary: true },
        { formula: 'B2', dbColumnName: 'companyName' },
        { formula: 'C2', dbColumnName: 'contactName' },
        { formula: 'D2', dbColumnName: 'contactTitle' },
        { formula: 'E2', dbColumnName: 'address' },
        { formula: 'F2', dbColumnName: 'region' },
        { formula: 'G2', dbColumnName: 'country' },
        { formula: 'H2', dbColumnName: 'city' },
        { formula: 'I2', dbColumnName: 'postalCode' },
        { formula: 'J2', dbColumnName: 'phone' },
        { formula: 'K2', dbColumnName: 'fax' },
    ],
};
templateSheet.setDataEntrySetting([customerRule]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataEntrySetting` | [`DataEntrySetting`](../modules/GC.Spread.Report.md#dataentrysetting) | 数据输入设置。 |

#### Returns

`void`

___

### <a id="setlayoutsetting" name="setlayoutsetting"></a> setLayoutSetting

▸ **setLayoutSetting**(`setting`): `void`

设置布局设置。

**`example`**
```
const dataManager = spread.dataManager();
dataManager.addTable("orders",
     {
          remote: {
              read: {
                  url: "https://demodata.grapecity.com/northwind/api/v1/Orders"
              }
          }
     }
);
templateSheet.setTemplateCell(1, 0, { type: 'List', binding: 'orders[orderId]' });
const setting = {
     dataRange: "A2",
     type: "RowLayout",
     rowCount: 10
}
templateSheet.setLayoutSetting(setting);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `setting` | [`LayoutSetting`](../modules/GC.Spread.Report.md#layoutsetting) | 布局设置。 |

#### Returns

`void`

___

### <a id="setpaginationsetting" name="setpaginationsetting"></a> setPaginationSetting

▸ **setPaginationSetting**(`setting`): `void`

设置分页设置。

**`example`**
```
// 设置纸张大小分页。
const printInfo = templateSheet.printInfo();
printInfo.paperSize().kind(GC.Spread.Sheets.Print.PaperKind.a4);
templateSheet.setPaginationSetting({
    paperSizePagination: true,
    titleRow: {
        start: 0,
        end: 0,
    },
    titleCol: {
        start: 0,
        end: 0,
    },
    paginationOrder: 'OverThenDown',
});

// 设置行分页，行分页仅适用于列表模板单元格。
templateSheet.setTemplateCell(1, 0, { type: 'List', binding: 'orders[orderId]' });
templateSheet.setPaginationSetting({
    rowPagination: {
        paginationDataCell: 'A2',
        rowCountPerPage: 20,
    },
    titleRow: {
        start: 0,
        end: 0,
    },
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `setting` | [`IPaginationSetting`](../interfaces/GC.Spread.Report.IPaginationSetting.md) | 分页设置。 |

#### Returns

`void`

___

### <a id="settemplatecell" name="settemplatecell"></a> setTemplateCell

▸ **setTemplateCell**(`row`, `col`, `templateCell`): `void`

设置模板单元格。

**`example`**
```
const dataManager = spread.dataManager();
dataManager.addTable("orders",
     {
          remote: {
              read: {
                  url: "https://demodata.grapecity.com/northwind/api/v1/Orders"
              }
          }
     }
);
// 设置 A2 单元格的模板单元格设置。
templateSheet.setTemplateCell(1, 0, { type: 'List', binding: 'orders[shipCity]' });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `templateCell` | [`TemplateCell`](../modules/GC.Spread.Report.md#templatecell) | 模板单元格。 |

#### Returns

`void`
