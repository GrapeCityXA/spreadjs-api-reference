# Class: ReportSheet

[Spread](../modules/GC.Spread.md).[Report](../modules/GC.Spread.Report.md).ReportSheet

## Table of contents

### Constructors

- [constructor](GC.Spread.Report.ReportSheet.md#constructor)

### Properties

- [options](GC.Spread.Report.ReportSheet.md#options)

### Methods

- [addRecordAt](GC.Spread.Report.ReportSheet.md#addrecordat)
- [bind](GC.Spread.Report.ReportSheet.md#bind)
- [currentPage](GC.Spread.Report.ReportSheet.md#currentpage)
- [deleteRecordAt](GC.Spread.Report.ReportSheet.md#deleterecordat)
- [generatePageSheets](GC.Spread.Report.ReportSheet.md#generatepagesheets)
- [getActualStyle](GC.Spread.Report.ReportSheet.md#getactualstyle)
- [getCells](GC.Spread.Report.ReportSheet.md#getcells)
- [getChanges](GC.Spread.Report.ReportSheet.md#getchanges)
- [getCollapseState](GC.Spread.Report.ReportSheet.md#getcollapsestate)
- [getColumnWidth](GC.Spread.Report.ReportSheet.md#getcolumnwidth)
- [getPagesCount](GC.Spread.Report.ReportSheet.md#getpagescount)
- [getRange](GC.Spread.Report.ReportSheet.md#getrange)
- [getRowHeight](GC.Spread.Report.ReportSheet.md#getrowheight)
- [getSpan](GC.Spread.Report.ReportSheet.md#getspan)
- [getStyle](GC.Spread.Report.ReportSheet.md#getstyle)
- [getTemplate](GC.Spread.Report.ReportSheet.md#gettemplate)
- [getTemplateCell](GC.Spread.Report.ReportSheet.md#gettemplatecell)
- [getValue](GC.Spread.Report.ReportSheet.md#getvalue)
- [isDirty](GC.Spread.Report.ReportSheet.md#isdirty)
- [loadTemplate](GC.Spread.Report.ReportSheet.md#loadtemplate)
- [name](GC.Spread.Report.ReportSheet.md#name)
- [parameter](GC.Spread.Report.ReportSheet.md#parameter)
- [printInfo](GC.Spread.Report.ReportSheet.md#printinfo)
- [printPageIndexes](GC.Spread.Report.ReportSheet.md#printpageindexes)
- [refresh](GC.Spread.Report.ReportSheet.md#refresh)
- [regenerateReport](GC.Spread.Report.ReportSheet.md#regeneratereport)
- [renderMode](GC.Spread.Report.ReportSheet.md#rendermode)
- [repaint](GC.Spread.Report.ReportSheet.md#repaint)
- [resetCellValue](GC.Spread.Report.ReportSheet.md#resetcellvalue)
- [setParametersUI](GC.Spread.Report.ReportSheet.md#setparametersui)
- [submit](GC.Spread.Report.ReportSheet.md#submit)
- [toWorksheet](GC.Spread.Report.ReportSheet.md#toworksheet)
- [toggleCollapseState](GC.Spread.Report.ReportSheet.md#togglecollapsestate)
- [unbind](GC.Spread.Report.ReportSheet.md#unbind)
- [updateCellValue](GC.Spread.Report.ReportSheet.md#updatecellvalue)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ReportSheet**(`name`)

表示 ReportSheet。

**`example`**
```
const spread = new GC.Spread.Sheets.Workbook('spread-host', { sheetCount: 0 });
const reportSheet = spread.addSheetTab(0, 'orders-report', GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = reportSheet.getTemplate();

const ordersTable = spread.dataManager().addTable('Orders', {
    remote: {
        read: {
            url: 'https://demodata.mescius.io/northwind/api/v1/orders'
        }
    }
});

// 从远程加载数据。
ordersTable.fetch().then(() => {
    // 设置模板样式。
    const headerStyle = new GC.Spread.Sheets.Style();
    headerStyle.backColor = '#80CBC4';
    headerStyle.foreColor = '#424242';
    headerStyle.hAlign = GC.Spread.Sheets.HorizontalAlign.right;
    headerStyle.font = '12px Maine';
    const dataStyle = new GC.Spread.Sheets.Style();
    dataStyle.foreColor = '#424242';
    dataStyle.hAlign = GC.Spread.Sheets.HorizontalAlign.right;
    dataStyle.font = '12px Maine';
    const border = new GC.Spread.Sheets.LineBorder('#E0E0E0', 1);
    dataStyle.borderBottom = border;
    dataStyle.borderTop = border;
    dataStyle.borderLeft = border;
    dataStyle.borderRight = border;
    const colWidthArray = [90, 90, 90, 80, 220, 150, 110];
    colWidthArray.forEach((width, i) => {
        templateSheet.setColumnWidth(i, width);
    });
    templateSheet.getRange('A1:G1').setStyle(headerStyle);
    templateSheet.getRange('A2:G2').setStyle(dataStyle);
    templateSheet.setFormatter(1, 2, 'yyyy-MM-dd');

    // set value and binding for the template.
    const columns = ['orderId', 'customerId', 'orderDate', 'freight', 'shipName', 'shipCity', 'shipCountry'];
    columns.forEach((columnName, i) => {
        templateSheet.setValue(0, i, `${columnName[0].toUpperCase()}${columnName.substring(1)}`);
        templateSheet.setTemplateCell(1, i, {
            type: 'List',
            binding: `Orders[${columnName}]`,
        });
    });

    reportSheet.refresh();
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | ReportSheet的名称。 |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`IReportOptions`](../interfaces/GC.Spread.Report.IReportOptions.md)

表示 ReportSheet 的选项。

**`property`** {GC.Spread.Sheets.Style} [dirtyStyle] 在预览模式下用于绘制修改单元格的样式。

**`property`** {boolean} [printAllPages] 是否打印所有页面。

## Methods

### <a id="addrecordat" name="addrecordat"></a> addRecordAt

▸ **addRecordAt**(`row`, `col`): `void`

根据指定单元格添加记录。

**`example`**
```
// 在 A2 单元格添加记录。
reportSheet.addRecordAt(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`void`

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `data?`, `fn?`): `void`

将事件绑定到报告表。

**`example`**
```
// 此示例将 ReportSheetDataChanged 事件绑定到报告表。
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetDataChanged, (event, args) => {
    let reportsheet = args.sheet, changes = reportsheet.getChanges();
    if (allowSubmit(changes)) { // users can submit or drop this changing.
         reportsheet.submit(); // submit changes.
    } else {
         reportsheet.refresh(); // drop changes.
    }
});
// 在 UI 中编辑/更新/删除记录后，将触发 ReportSheetDataChanged 事件。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `data?` | `any` | 可选。指定要传递给函数的附加数据。 |
| `fn?` | `Function` | 指定在事件发生时运行的函数。 |

#### Returns

`void`

___

### <a id="currentpage" name="currentpage"></a> currentPage

▸ **currentPage**(`page?`): `number`

获取或设置当前页面索引。

**`example`**
```
// 获取当前页面索引。
const page = reportSheet.currentPage();

// 转到下一页。
reportSheet.currentPage(page + 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `page?` | `number` | 页面索引（0 基）。 |

#### Returns

`number`

返回当前页面索引。

___

### <a id="deleterecordat" name="deleterecordat"></a> deleteRecordAt

▸ **deleteRecordAt**(`row`, `col`): `void`

根据指定单元格删除记录。

**`example`**
```
// 删除 A2 单元格的记录。
reportSheet.deleteRecordAt(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`void`

___

### <a id="generatepagesheets" name="generatepagesheets"></a> generatePageSheets

▸ **generatePageSheets**(`addToSpread`, `sheetNameGenerator?`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)[]

将当前报告的每个页面生成一个工作表，并返回它们组成的数组。

**`example`**
```
// 生成页面并添加到工作表。
const pageSheets = reportSheet.generatePageSheets(true);

// 生成页面并添加到工作表，并自定义工作表名称。
const pageSheets = reportSheet.generatePageSheets(true, (i) => `report-page-${i + 1}`);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `addToSpread` | `boolean` | 控制是否将页面工作表添加到当前工作表。 |
| `sheetNameGenerator?` | [`SheetNameGenerator`](../modules/GC.Spread.Report.md#sheetnamegenerator) | 可选的工作表名称生成器。 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)[]

返回生成的页面工作表。

___

### <a id="getactualstyle" name="getactualstyle"></a> getActualStyle

▸ **getActualStyle**(`row`, `col`): [`Style`](GC.Spread.Sheets.Style.md)

获取当前渲染模式下的单元格实际样式。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.getCell(0, 0).backColor("red");
templateSheet.setTemplateCell(1, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.getCell(1, 0).backColor("green");
const designActualStyle1 = report.getActualStyle(0, 0); // backColor: red
const designActualStyle2 = report.getActualStyle(1, 0); // backColor: green
report.renderMode("Preview");
const previewActualStyle1 = report.getActualStyle(0, 0); // backColor: red
const previewActualStyle2 = report.getActualStyle(1, 0); // backColor: red
report.renderMode("PaginatedPreview");
const paginatedPreviewActualStyle1 = report.getActualStyle(0, 0); // backColor: red
const paginatedPreviewActualStyle2 = report.getActualStyle(1, 0); // backColor: red
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回当前渲染模式下的单元格实际样式。

___

### <a id="getcells" name="getcells"></a> getCells

▸ **getCells**(`templateRow`, `templateCol`, `currentRow?`, `currentCol?`): [`IDataCell`](../interfaces/GC.Spread.Report.IDataCell.md)[]

获取当前单元格在预览模式下的展开单元格。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setTemplateCell(1, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
report.regenerateReport();
const allCustomerIdCells = report.getCells(0, 0); // all 89 cells
const fistCustomerIdCell = report.getCells(0, 0, 0, 0); // value: VINET
const allOrderIdCells = report.getCells(1, 0); // all 830 cells
const firstOrderIdCell = report.getCells(1, 0, 89, 0); // value: 10248
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `templateRow` | `number` | 模板中的行索引。 |
| `templateCol` | `number` | 模板中的列索引。 |
| `currentRow?` | `number` | 当前单元格在预览中的行索引。 |
| `currentCol?` | `number` | 当前单元格在预览中的列索引。 |

#### Returns

[`IDataCell`](../interfaces/GC.Spread.Report.IDataCell.md)[]

返回当前单元格在预览模式下的展开单元格。

___

### <a id="getchanges" name="getchanges"></a> getChanges

▸ **getChanges**(): [`Change`](../modules/GC.Spread.Report.md#change)[]

返回报告表数据条目模式更新插入和删除数据更改。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   showCollapseButton: true
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.updateCellValue(0, 1, "test");
report.addRecordAt(1, 0);
report.updateCellValue(2, 0, 111);
report.updateCellValue(2, 1, "test2");
report.deleteRecordAt(3, 0);
report.getChanges(); // 一个删除记录和两个更新记录。
```

#### Returns

[`Change`](../modules/GC.Spread.Report.md#change)[]

返回报告表更新插入和删除数据更改。

___

### <a id="getcollapsestate" name="getcollapsestate"></a> getCollapseState

▸ **getCollapseState**(`row`, `col`): `boolean`

返回指定单元格的折叠状态。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   showCollapseButton: true
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.addSpan(0, 0, 2, 1);
report.renderMode("Preview");
report.getCollapseState(0, 0); // false
report.toggleCollapseState(0, 0);
report.getCollapseState(0, 0); // true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`boolean`

___

### <a id="getcolumnwidth" name="getcolumnwidth"></a> getColumnWidth

▸ **getColumnWidth**(`col`): `number`

获取指定列的列宽。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   spillDirection: "Horizontal"
});
templateSheet.setColumnWidth(0, 100);
const designColumnWidth1 = report.getColumnWidth(0); // ColumnWidth: 100
const designColumnWidth2 = report.getColumnWidth(1); // ColumnWidth: 62
report.renderMode("Preview");
const previewColumnWidth1 = report.getColumnWidth(0); // ColumnWidth: 100
const previewColumnWidth2 = report.getColumnWidth(1); // ColumnWidth: 100
report.renderMode("PaginatedPreview");
const paginatedPreviewColumnWidth1 = report.getColumnWidth(0); // ColumnWidth: 100
const paginatedPreviewColumnWidth2 = report.getColumnWidth(1); // ColumnWidth: 100
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |

#### Returns

`number`

返回列宽。

___

### <a id="getpagescount" name="getpagescount"></a> getPagesCount

▸ **getPagesCount**(): `number`

获取报告的页面数量。

**`example`**
```
// 获取页面数量。
const pagesCount = reportSheet.getPagesCount();
```

#### Returns

`number`

返回报告的页面数量。

___

### <a id="getrange" name="getrange"></a> getRange

▸ **getRange**(): [`Range`](GC.Spread.Sheets.Range.md)

返回报告表范围。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(199, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
const designRange = report.getRange(); // row: 0, col: 0, rowCount: 200, colCount: 20.
report.renderMode("Preview");
const previewRange = report.getRange(); // row: 0, col: 0, rowCount: 288, colCount: 1.
report.renderMode("PaginatedPreview");
const paginatedPreviewRange = report.getRange(); // row: 0, col: 0, rowCount: 45, colCount: 1.
```

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

返回报告表范围。
如果渲染模式为设计，返回模板表范围。
如果渲染模式为预览，返回整个报告范围。
如果渲染模式为分页预览，返回当前页的范围。

___

### <a id="getrowheight" name="getrowheight"></a> getRowHeight

▸ **getRowHeight**(`row`): `number`

获取指定行的高度。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setRowHeight(0, 30);
const designRowHeight1 = report.getRowHeight(0); // RowHeight: 30
const designRowHeight2 = report.getRowHeight(1); // RowHeight: 20
report.renderMode("Preview");
const previewRowHeight1 = report.getRowHeight(0); // RowHeight: 30
const previewRowHeight2 = report.getRowHeight(1); // RowHeight: 30
report.renderMode("PaginatedPreview");
const paginatedPreviewRowHeight1 = report.getRowHeight(0); // RowHeight: 30
const paginatedPreviewRowHeight2 = report.getRowHeight(1); // RowHeight: 30
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`number`

返回行高。

___

### <a id="getspan" name="getspan"></a> getSpan

▸ **getSpan**(`row`, `col`): [`Range`](GC.Spread.Sheets.Range.md)

获取当前渲染模式下的单元格范围。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.addSpan(0, 0, 2, 1);
const designSpan1 = report.getSpan(0, 0); // span: row: 0, col: 0, rowCount: 2, colCount: 1
const designSpan2 = report.getSpan(2, 0); // span: null
report.renderMode("Preview");
const previewSpan1 = report.getSpan(0, 0); // span: row: 0, col: 0, rowCount: 2, colCount: 1
const previewSpan2 = report.getSpan(2, 0); // span: row: 2, col: 0, rowCount: 2, colCount: 1
report.renderMode("PaginatedPreview");
const paginatedPreviewSpan1 = report.getSpan(0, 0); // span: row: 0, col: 0, rowCount: 2, colCount: 1
const paginatedPreviewSpan2 = report.getSpan(2, 0); // span: row: 2, col: 0, rowCount: 2, colCount: 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

返回单元格的范围。

___

### <a id="getstyle" name="getstyle"></a> getStyle

▸ **getStyle**(`row`, `col`): [`Style`](GC.Spread.Sheets.Style.md)

获取当前渲染模式下的单元格样式。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.getCell(0, 0).backColor("red");
templateSheet.setTemplateCell(1, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.getCell(1, 0).backColor("green");
const designStyle1 = report.getStyle(0, 0); // backColor: red
const designStyle2 = report.getStyle(1, 0); // backColor: green
report.renderMode("Preview");
const previewStyle1 = report.getStyle(0, 0); // backColor: red
const previewStyle2 = report.getStyle(1, 0); // backColor: red
report.renderMode("PaginatedPreview");
const paginatedPreviewStyle1 = report.getStyle(0, 0); // backColor: red
const paginatedPreviewStyle2 = report.getStyle(1, 0); // backColor: red
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回单元格的样式。

___

### <a id="gettemplate" name="gettemplate"></a> getTemplate

▸ **getTemplate**(): [`TemplateSheet`](GC.Spread.Report.TemplateSheet.md)

获取当前报告表的模板表。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate(); // 获取报告表的模板表
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
report.renderMode("Preview");
```

#### Returns

[`TemplateSheet`](GC.Spread.Report.TemplateSheet.md)

返回当前报告表的模板表。

___

### <a id="gettemplatecell" name="gettemplatecell"></a> getTemplateCell

▸ **getTemplateCell**(`row`, `col`): [`TemplateCell`](../modules/GC.Spread.Report.md#templatecell)

获取指定单元格的模板单元格。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setTemplateCell(1, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
const designTemplateCell1 = report.getTemplateCell(0, 0); // binding: Orders[customerId]
const designTemplateCell2 = report.getTemplateCell(1, 0); // binding: Orders[orderId]
report.renderMode("Preview");
const previewTemplateCell1 = report.getTemplateCell(0, 0); // binding: Orders[customerId]
const previewTemplateCell2 = report.getTemplateCell(1, 0); // binding: Orders[customerId]
const previewTemplateCell3 = report.getTemplateCell(89, 0); // binding: Orders[orderId]
report.renderMode("PaginatedPreview");
const paginatedPreviewTemplateCell1 = report.getTemplateCell(0, 0); // binding: Orders[customerId]
const paginatedPreviewTemplateCell2 = report.getTemplateCell(1, 0); // binding: Orders[customerId]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`TemplateCell`](../modules/GC.Spread.Report.md#templatecell)

返回指定单元格的模板单元格。
如果渲染模式为设计，返回指定单元格的模板单元格。
如果渲染模式为预览，返回指定单元格的模板单元格。
如果渲染模式为分页预览，返回指定单元格的模板单元格。

___

### <a id="getvalue" name="getvalue"></a> getValue

▸ **getValue**(`row`, `col`): `any`

获取当前渲染模式下的单元格值。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setValue(1, 0, "test");
const designValue = report.getValue(1, 0); // test
report.renderMode("Preview");
const previewValue = report.getValue(1, 0); // TOMSP
report.renderMode("PaginatedPreview");
const paginatedPreviewValue = report.getValue(1, 0); // TOMSP
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`any`

返回单元格的值。

___

### <a id="isdirty" name="isdirty"></a> isDirty

▸ **isDirty**(): `boolean`

返回一个布尔值，指示报告是否具有未提交的更改。

**`example`**
```
// 如果当前报告表具有未提交的更改，isDirty 将为 true。
const isDirty = reportSheet.isDirty();
```

#### Returns

`boolean`

如果报告具有未提交的更改，则返回 true，否则返回 false。

___

### <a id="loadtemplate" name="loadtemplate"></a> loadTemplate

▸ **loadTemplate**(`templateJson`): `void`

更新报告表模板，报告也将根据新模板和参数值重新生成。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = new GC.Spread.Report.TemplateSheet("Template");
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
report.loadTemplate(templateSheet.toJSON());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `templateJson` | `Object` | 模板 json。 |

#### Returns

`void`

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置报告表的名称。

**`example`**
```
// 获取报告表的名称
const name = reportSheet.name();

// 设置报告表的名称
reportSheet.name('new-name');
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

返回报告表的名称。

___

### <a id="parameter" name="parameter"></a> parameter

▸ **parameter**(`parameter?`): [`IParameter`](../interfaces/GC.Spread.Sheets.IParameter.md)

获取或设置报告表的参数。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
report.getTemplate().setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   filter: {
       condition: {
           column: "customerId",
           operator: "Equal",
           parameter: "customerId"
       }
   }
});
report.renderMode("Preview");

let parameter = report.parameter(); // 获取报告表的参数
parameter.customerId = "VINET";
report.parameter(parameter); // 设置参数。
report.regenerateReport(); // 根据新参数重新生成报告表。
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `parameter?` | [`IParameter`](../interfaces/GC.Spread.Sheets.IParameter.md) |

#### Returns

[`IParameter`](../interfaces/GC.Spread.Sheets.IParameter.md)

返回报告表当前工作参数。

___

### <a id="printinfo" name="printinfo"></a> printInfo

▸ **printInfo**(`value?`): [`ReportSheet`](GC.Spread.Report.ReportSheet.md) \| [`PrintInfo`](GC.Spread.Sheets.Print.PrintInfo.md)

获取或设置报告表的打印信息。

**`example`**
```
// 设置纸张大小。
const printInfo = reportSheet.printInfo();
printInfo.paperSize(new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a3));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintInfo`](GC.Spread.Sheets.Print.PrintInfo.md) |

#### Returns

[`ReportSheet`](GC.Spread.Report.ReportSheet.md) \| [`PrintInfo`](GC.Spread.Sheets.Print.PrintInfo.md)

如果未设置值，则返回报告表的打印信息；否则，返回报告表。

___

### <a id="printpageindexes" name="printpageindexes"></a> printPageIndexes

▸ **printPageIndexes**(`pageIndexes?`): `number`[]

获取或设置要打印的页面索引数组。空数组表示打印所有页面。

**`example`**
```
// 打印当前报告的第一个和第五个页面。
reportSheet.printPageIndexes([0, 4]);
reportSheet.options.printAllPages = true;
spread.print();

// 清除打印页面索引设置。
reportSheet.printPageIndexes([]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pageIndexes?` | `number`[] | 要打印的页面索引数组（0 基）。 |

#### Returns

`number`[]

返回要打印的页面索引数组。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新当前报告表，所有渲染模式都支持此功能。
设计：刷新模板表的缓存并重新绘制。
预览：根据当前模板表重新生成报告并重新绘制。
分页预览：根据当前模板表重新生成报告并重新绘制。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
report.refresh();
```

#### Returns

`void`

___

### <a id="regeneratereport" name="regeneratereport"></a> regenerateReport

▸ **regenerateReport**(): `void`

根据当前模板重新生成报告。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
report.regenerateReport();
```

#### Returns

`void`

___

### <a id="rendermode" name="rendermode"></a> renderMode

▸ **renderMode**(`renderMode?`): [`RenderMode`](../modules/GC.Spread.Report.md#rendermode)

获取或设置渲染模式。

**`example`**
```
// 切换到设计模式。
reportSheet.renderMode('Design');

// 切换到预览模式。
reportSheet.renderMode('Preview');

// 切换到分页预览模式。
reportSheet.renderMode('PaginatedPreview');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderMode?` | [`RenderMode`](../modules/GC.Spread.Report.md#rendermode) | 渲染模式。 |

#### Returns

[`RenderMode`](../modules/GC.Spread.Report.md#rendermode)

返回渲染模式。

___

### <a id="repaint" name="repaint"></a> repaint

▸ **repaint**(): `void`

重新绘制当前报告表。

#### Returns

`void`

___

### <a id="resetcellvalue" name="resetcellvalue"></a> resetCellValue

▸ **resetCellValue**(`row`, `col`): `void`

重置指定单元格的值。

**`example`**
```
// 如果 A2 单元格的值被修改，resetCellValue 可以重置 A2 单元格到其原始值。
reportSheet.resetCellValue(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`void`

___

### <a id="setparametersui" name="setparametersui"></a> setParametersUI

▸ **setParametersUI**(`host`, `initParametersUI`, `onChange`): `void`

设置报告表的参数UI。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
report.parameter({ customerId: "VINET" });
report.getTemplate().setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   filter: {
       condition: {
           column: "customerId",
           operator: "Equal",
           parameter: "customerId"
       }
   }
});
report.renderMode("Preview");

const host = document.getElementById("parameterUIHost");
report.setParametersUI(host, initParametersUI, onChanged);
function initParametersUI (sheet) {
    sheet.getCell(3, 3).value("CustomerId:"); // 添加静态标签单元格
    sheet.getCell(3, 4).bindingPath("customerId").tag("customerId"); // 添加参数绑定路径和标签到此单元格
    const submitButton = new GC.Spread.Sheets.CellTypes.Button(); // 添加提交按钮
    submitButton.text("Submit");
    sheet.getCell(3, 5).cellType(submitButton).tag("submitButton"); // 设置按钮单元格类型和标签到此单元格
}
function onChanged (reportSheet, changedArgs) {
    if (changedArgs.tag === "submitButton") { // 提交按钮点击。
        reportSheet.regenerateReport();
    }
    if (changedArgs.tag === "customerId") {
        changedArgs.newValue = changedArgs.newValue.toUpperCase(); // 更新 newValue 这里。
    }
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 参数UI宿主元素或宿主ID。 |
| `initParametersUI` | [`InitParametersUIFunctionType`](../modules/GC.Spread.Report.md#initparametersuifunctiontype) | 修改参数UI表的回调。 |
| `onChange` | [`OnChangeFunctionType`](../modules/GC.Spread.Report.md#onchangefunctiontype) | 参数UI值更改或按钮点击时的回调。 |

#### Returns

`void`

___

### <a id="submit" name="submit"></a> submit

▸ **submit**(): `void`

通过 DataManger 提交更改到远程数据库。

**`example`**
```
// 提交更改。
reportSheet.submit();
```

#### Returns

`void`

___

### <a id="toworksheet" name="toworksheet"></a> toWorksheet

▸ **toWorksheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

根据当前报告表生成一个静态工作表（没有公式，没有单元格绑定）。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
});
report.renderMode("Preview");
const reportWorksheet = report.toWorksheet();
```

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

返回生成的工作表。

___

### <a id="togglecollapsestate" name="togglecollapsestate"></a> toggleCollapseState

▸ **toggleCollapseState**(`row`, `col`, `targetState?`, `recursive?`): `void`

切换指定单元格的折叠状态。

**`example`**
```
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[customerId]",
   type: "Group",
   showCollapseButton: true
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.addSpan(0, 0, 2, 1);
report.renderMode("Preview");
report.toggleCollapseState(0, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `targetState?` | ``"Expanded"`` \| ``"Collapsed"`` | 目标状态，折叠或展开特定单元格。 |
| `recursive?` | `boolean` | 如果为 true，将更新当前单元格及其所有后代单元格的状态，如果为 false，则只更新当前单元格。 |

#### Returns

`void`

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

移除报告表的事件绑定。

**`example`**
```
// 此示例在第一次数据更改后取消绑定 ReportSheetDataChanged 事件。
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetDataChanged, (event, args) => {
    let reportsheet = args.sheet, changes = reportsheet.getChanges();
    console.log(changes);
    reportsheet.unbind(GC.Spread.Sheets.Events.ReportSheetDataChanged);
});
// 在 UI 中编辑/更新/删除记录后，将触发 ReportSheetDataChanged 事件。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `fn?` | `Function` | 指定要移除绑定的函数。 |

#### Returns

`void`

___

### <a id="updatecellvalue" name="updatecellvalue"></a> updateCellValue

▸ **updateCellValue**(`row`, `col`, `value`): `void`

更新指定单元格的值。

**`example`**
```
// 更新 A2 单元格的值。
reportSheet.updateCellValue(1, 0, 'test');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `any` | 单元格的新值。 |

#### Returns

`void`
