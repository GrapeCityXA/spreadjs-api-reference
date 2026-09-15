# Interface: IReportSheetRecordsSubmittedEventArgs

[Spread](../modules/GC.Spread.md).[Report](../modules/GC.Spread.Report.md).IReportSheetRecordsSubmittedEventArgs

## Table of contents

### Properties

- [deleteFailedRecords](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#deletefailedrecords)
- [deleteSuccessRecords](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#deletesuccessrecords)
- [sheet](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#sheet)
- [sheetName](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#sheetname)
- [updateFailedRecords](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#updatefailedrecords)
- [updateSuccessRecords](GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md#updatesuccessrecords)

## Properties

### <a id="deletefailedrecords" name="deletefailedrecords"></a> deleteFailedRecords

• **deleteFailedRecords**: [`IFailedRecord`](GC.Spread.Report.IFailedRecord.md)[]

___

### <a id="deletesuccessrecords" name="deletesuccessrecords"></a> deleteSuccessRecords

• **deleteSuccessRecords**: [`IRecord`](GC.Spread.Report.IRecord.md)[]

包括已删除的记录。

___

### <a id="sheet" name="sheet"></a> sheet

• **sheet**: [`ReportSheet`](../classes/GC.Spread.Report.ReportSheet.md)

___

### <a id="sheetname" name="sheetname"></a> sheetName

• **sheetName**: `string`

___

### <a id="updatefailedrecords" name="updatefailedrecords"></a> updateFailedRecords

• **updateFailedRecords**: [`IFailedRecord`](GC.Spread.Report.IFailedRecord.md)[]

___

### <a id="updatesuccessrecords" name="updatesuccessrecords"></a> updateSuccessRecords

• **updateSuccessRecords**: [`IRecord`](GC.Spread.Report.IRecord.md)[]

包括更新和插入的记录。
