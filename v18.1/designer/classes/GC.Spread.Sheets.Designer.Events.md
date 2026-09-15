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

定义SpreadJS设计器支持的事件。

## Events

### <a id="fileloaded" name="fileloaded"></a> FileLoaded

• `Static` **FileLoaded**: `string`

当通过Spread.Sheets.Designer文件操作完成文件加载时触发。

**`name`** GC.Spread.Sheets.Designer#FileLoaded

**`param`** *[GC.Spread.Sheets.Designer](../modules/GC.Spread.Sheets.Designer.md)* `designer` 触发事件的设计器实例。

**`param`** *[GC.Spread.Sheets.Designer.FileType](../enums/GC.Spread.Sheets.Designer.FileType.md)* `fileType` 导入的文件类型。

**`example`**
```
// 此示例使用FileLoaded事件。
let designer = GC.Spread.Sheets.Designer.findControl(document.getElementById("gc-designer-container"));
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, (event, data)=>{
  console.log("文件已加载");
 });
```

___

### <a id="fileloading" name="fileloading"></a> FileLoading

• `Static` **FileLoading**: `string`

当通过Spread.Sheets.Designer文件操作开始加载文件时触发。

**`name`** GC.Spread.Sheets.Designer#FileLoading

**`param`** *[GC.Spread.Sheets.Designer](../modules/GC.Spread.Sheets.Designer.md)* `designer` 触发事件的设计器实例。

**`param`** *[GC.Spread.Sheets.Designer.FileType](../enums/GC.Spread.Sheets.Designer.FileType.md)* `fileType` 导入的文件类型。

**`param`** *string* `fileName` 导入的文件名。

**`param`** *Object | string* `data` 来自文件的JSON数据、CSV数据或原始文件数据。

**`param`** *boolean* `cancel` 指示是否取消操作的布尔值。

**`example`**
```
// 此示例使用FileLoading事件。
let designer = GC.Spread.Sheets.Designer.findControl(document.getElementById("gc-designer-container"));
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoading, (event, data)=>{
  console.log("文件正在加载");
 });
```
