# Class: Events

[Sheets](../modules/GC.Spread.Sheets.md).[Designer](../modules/GC.Spread.Sheets.Designer.md).Events

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Designer.Events.md#constructor)

### Events

- [FileLoaded](GC.Spread.Sheets.Designer.Events.md#fileloaded)
- [FileLoading](GC.Spread.Sheets.Designer.Events.md#fileloading)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Events**()

SpreadJS 设计器中支持的事件

## Events

### <a id="fileloaded" name="fileloaded"></a> FileLoaded

• `Static` **FileLoaded**: `string`

Spread.Sheets.Designer文件加载完成时触发

**`name`** GC.Spread.Sheets.Designer#FileLoaded

**`param`** *[GC.Spread.Sheets.Designer](../modules/GC.Spread.Sheets.Designer.md)* `designer` 触发事件的设计器实例

**`param`** *[GC.Spread.Sheets.Designer.FileType](../enums/GC.Spread.Sheets.Designer.FileType.md)* `fileType` 导入文件类型

**`代码示例`**
```
//使用FileLoaded事件示例
let designer = GC.Spread.Sheets.Designer.findControl(document.getElementById("gc-designer-container"));
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, (event, data)=>{
  console.log("file has loaded");
 });
```

___

### <a id="fileloading" name="fileloading"></a> FileLoading

• `Static` **FileLoading**: `string`

Spread.Sheets.Designer文件加载时触发

**`name`** GC.Spread.Sheets.Designer#FileLoading

**`param`** *[GC.Spread.Sheets.Designer](../modules/GC.Spread.Sheets.Designer.md)* `designer` 触发事件的设计器实例

**`param`** *[GC.Spread.Sheets.Designer.FileType](../enums/GC.Spread.Sheets.Designer.FileType.md)* `fileType` 导入文件类型

**`param`** *string* `fileName` 导入文件名。

**`param`** *Object | string* `data` 来自文件 json 数据或 csv 数据或原始文件的数据。

**`param`** *boolean* `cancel` 指示是否应取消操作的值.

**`example`**
```
//此示例使用FileLoading事件
let designer = GC.Spread.Sheets.Designer.findControl(document.getElementById("gc-designer-container"));
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoading, (event, data)=>{
  console.log("file is loading");
 });
```
