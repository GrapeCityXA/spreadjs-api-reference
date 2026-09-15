# Class: Designer

[Sheets](../modules/GC.Spread.Sheets.md).[Designer](../modules/GC.Spread.Sheets.Designer.md).Designer

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Designer.Designer.md#constructor)

### Methods

- [activeRibbonTab](GC.Spread.Sheets.Designer.Designer.md#activeribbontab)
- [bind](GC.Spread.Sheets.Designer.Designer.md#bind)
- [destroy](GC.Spread.Sheets.Designer.Designer.md#destroy)
- [getData](GC.Spread.Sheets.Designer.Designer.md#getdata)
- [getWorkbook](GC.Spread.Sheets.Designer.Designer.md#getworkbook)
- [refresh](GC.Spread.Sheets.Designer.Designer.md#refresh)
- [setConfig](GC.Spread.Sheets.Designer.Designer.md#setconfig)
- [setData](GC.Spread.Sheets.Designer.Designer.md#setdata)
- [setWorkbook](GC.Spread.Sheets.Designer.Designer.md#setworkbook)
- [unbind](GC.Spread.Sheets.Designer.Designer.md#unbind)
- [unbindAll](GC.Spread.Sheets.Designer.Designer.md#unbindall)
- [RegisterComponent](GC.Spread.Sheets.Designer.Designer.md#registercomponent)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Designer**(`host`, `config?`, `spread?`, `spreadOptions?`)

使用指定的DOM元素、自定义配置和spread组成设计器

**`代码示例`**
```
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var customConfig = {
      ribbon: [
          {
              id: "home",
              text: "HOME",
              buttonGroups: [
                {
                  label: "Undo",
                  thumbnailClass: "ribbon-thumbnail-undoRedo",
                  commandGroup: {
                    children: [
                      {
                        direction: "vertical",
                        commands: [
                          "undo",
                          "redo"
                        ]
                      }
                    ]
                  }
                }
              ]
          }
      ],
      contextMenu: [
          "contextMenuCut",
          "contextMenuCopy",
      ],
      fileMenu: "fileMenuButton",
      sidePanels: [
          {
              position: "top",
              allowResize: true,
              command: "formulaBarPanel",
              uiTemplate: "formulaBarTemplate"
          },
      ]
 };
var customDesigner = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv2"), customConfig);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLDivElement` | 设计器的宿主 |
| `config?` | [`IDesignerConfig`](../interfaces/GC.Spread.Sheets.Designer.IDesignerConfig.md) | 设计器配置对象 |
| `spread?` | `Object` | 工作簿实例 |
| `spreadOptions?` | `Object` | 工作簿初始化选项 |

## Methods

### <a id="activeribbontab" name="activeribbontab"></a> activeRibbonTab

▸ **activeRibbonTab**(`ribbonTabId?`): `string`

获取或设置设计师活动的功能区选项卡 ID，功能区选项卡 ID 位于 DefaultConfig 中

**`example`**
```
// This example will set the designer active ribbon tab after designer initializing.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), undefined, spread);
let currentActiveRibbonTab = designer.activeRibbonTab(); // get the active ribbon tab id.
if (currentActiveRibbonTab !== "insert") {
    designer.activeRibbonTab("insert"); // will set the INSERT ribbon tab active.
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ribbonTabId?` | `string` | 新的活动功能区选项卡 ID |

#### Returns

`string`

- The designer current active ribbon tab id.

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `fn?`): `void`

将事件绑定到设计器

**`代码示例`**
```
//绑定事件示例
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoading, function(type, message){
    if (message.fileType = GC.Spread.Sheets.Designer.FileType.Excel){
        let spreadJsonData = message.data;
        if(spreadJsonData.sheetCount >= 3) {
             message.cancel = true;
        }
    };
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型 |
| `fn?` | `any` | 事件触发时要执行的函数 |

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁设计器并解除所有事件的绑定

**`代码示例`**
```
// 本示例将在创建新的设计器后销毁原设计器
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
designer.destroy();
```

#### Returns

`void`

___

### <a id="getdata" name="getdata"></a> getData

▸ **getData**(`key`): `any`

获取状态或值时，有两种类型的数据，一种是只在一个组件中使用的本地数据
另一个是全局数据，在整个设计器环境中使用，designer,getData (key)可以通过key获得存储在设计器中的全局数据

**`代码示例`**
```
// 本示例将在一个位置(如ribbon->Home)设置全局数据，并在另一个位置(如ribbon->setting)获取该全局数据，两个位置都有设计器实例
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var config = GC.Spread.Sheets.Designer.DefaultConfig;
var logInCommand = {
	title: "Login",
	text: "Login",
	iconClass: "ribbon-button-login",
	bigButton: true,
	commandName: "login",
	execute: (context, propertyName) => {
		alert('Log in new designer.');
		context.setData("isLogIn", true); // setData()
	 }
};
var getGiftCommand = {
	 title: "Get gift",
	 text: "Get gift",
	 iconClass: "ribbon-button-get-gift",
	 bigButton: 'true',
	 commandName: "getGift",
	 execute: (context, propertyName) => {
		 let isLogIn = context.getData("isLogIn"); // getData()
		 if (isLogIn) {
			 alert("Get gift");
		 }
		 else {
			 alert("Please log in");
		 }
	 }
};
config.commandMap = {
	 login: logInCommand,
	 getGift: getGiftCommand,
};
var logInCommandGroup = {
	 label: "Login",
	 thumbnailClass: "Login",
	 commandGroup: {
		 children: [
			 {
				 direction: "vertical",
				 commands: [
					 "Login"
				 ]
			 }
		 ]
	 }
};
var getGiftCommandGroup = {
	 label: "Gift",
	 thumbnailClass: "Gift",
	 commandGroup: {
		 children: [
			 {
				 direction: "vertical",
				 commands: [
					 "getGift"
				 ]
			 }
		 ]
	  }
 };
 if (config && config.ribbon) {
 config.ribbon[0].buttonGroups.unshift(logInCommandGroup);
 config.ribbon[5].buttonGroups.unshift(getGiftCommandGroup);
 }
 var d = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config, spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | 数据名称，唯一标识一个状态数据 |

#### Returns

`any`

- 该数据名称的值或状态可以是对象、字符串或其他类型

___

### <a id="getworkbook" name="getworkbook"></a> getWorkbook

▸ **getWorkbook**(): `Object`

获取设计器的工作簿

**`代码示例`**
```
// 本示例将获取设计器的工作簿
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var workbook = designer.getWorkbook();
var sheet = workbook.getActiveSheet();
```

#### Returns

`Object`

设计器的工作簿

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新设计器布局和功能区

**`代码示例`**
```
// 本示例将在更改设计器内容HTMLElement的大小后刷新设计器和功能区
var designerContent = document.getElementById("gc-designer-container");
designerContent.style.width =width + "px";
designerContent.style.height = height + "px";
designer.refresh();
```

#### Returns

`void`

___

### <a id="setconfig" name="setconfig"></a> setConfig

▸ **setConfig**(`config`): `void`

表示使用自定义配置的新设计器

**`代码示例`**
```
// 本示例将为现有设计器设置自定义配置
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var config = {
      ribbon: [
          {
              id: "home",
              text: "HOME",
              buttonGroups: [
                {
                  label: "Undo",
                  thumbnailClass: "ribbon-thumbnail-undoRedo",
                  commandGroup: {
                    children: [
                      {
                        direction: "vertical",
                        commands: [
                          "undo",
                          "redo"
                        ]
                      }
                    ]
                  }
                }
              ]
          }
      ],
      contextMenu: [
          "contextMenuCut",
          "contextMenuCopy",
      ],
      fileMenu: "fileMenuButton",
      sidePanels: [
          {
              position: "top",
              allowResize: true,
              command: "formulaBarPanel",
              uiTemplate: "formulaBarTemplate"
          },
      ]
 };
designer.setConfig(config);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `config` | [`IDesignerConfig`](../interfaces/GC.Spread.Sheets.Designer.IDesignerConfig.md) | 设计器配置对象 |

#### Returns

`void`

___

### <a id="setdata" name="setdata"></a> setData

▸ **setData**(`key`, `value`): `void`

设置状态或值时，有两种类型的数据，一种是只在一个组件中使用的本地数据
另一个是全局数据在整个设计环境中使用setData(key, value)可以通过具有设计器实例中的键值设置存储在设计器中的全局数据

**`代码示例`**
```
// 本示例将在一个位置(如ribbon->Home)设置全局数据，并在另一个位置(如ribbon->setting)获取该全局数据，两个位置都有设计器实例
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var config = GC.Spread.Sheets.Designer.DefaultConfig;
var logInCommand = {
	title: "Login",
	text: "Login",
	iconClass: "ribbon-button-login",
	bigButton: true,
	commandName: "login",
	execute: (context, propertyName) => {
		alert('Log in new designer.');
		context.setData("isLogIn", true); // setData()
	 }
};
var getGiftCommand = {
	 title: "Get gift",
	 text: "Get gift",
	 iconClass: "ribbon-button-get-gift",
	 bigButton: 'true',
	 commandName: "getGift",
	 execute: (context, propertyName) => {
		 let isLogIn = context.getData("isLogIn"); // getData()
		 if (isLogIn) {
			 alert("Get gift");
		 }
		 else {
			 alert("Please log in");
		 }
	 }
};
config.commandMap = {
	 login: logInCommand,
	 getGift: getGiftCommand,
};
var logInCommandGroup = {
	 label: "Login",
	 thumbnailClass: "Login",
	 commandGroup: {
		 children: [
			 {
				 direction: "vertical",
				 commands: [
					 "Login"
				 ]
			 }
		 ]
	 }
};
var getGiftCommandGroup = {
	 label: "Gift",
	 thumbnailClass: "Gift",
	 commandGroup: {
		 children: [
			 {
				 direction: "vertical",
				 commands: [
					 "getGift"
				 ]
			 }
		 ]
	  }
 };
 if (config && config.ribbon) {
 config.ribbon[0].buttonGroups.unshift(logInCommandGroup);
 config.ribbon[5].buttonGroups.unshift(getGiftCommandGroup);
 }
 var d = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config, spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | 数据名称，唯一标识一个状态数据，如果您多次使用不同的值设置相同的键，将只存储最新的值 |
| `value` | `any` | 该数据名称的值或状态可以是对象、字符串或其他类型 |

#### Returns

`void`

___

### <a id="setworkbook" name="setworkbook"></a> setWorkbook

▸ **setWorkbook**(`spread`): `void`

使用现有spread传入设计器

**`代码示例`**
```
// 这个例子将一个现有的spread设置到设计器
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
designer.setWorkbook(spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `spread` | `Object` | 现有的spread对象，用来取代设计器默认的spread |

#### Returns

`void`

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

移除事件与设计器的绑定

**`代码示例`**
```
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, function(event,data){
    console.log("file has loaded")
});
designer.unbind(GC.Spread.Sheets.Designer.Events.FileLoaded);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型 |
| `fn?` | `any` | 要移除其绑定的函数 |

#### Returns

`void`

___

### <a id="unbindall" name="unbindall"></a> unbindAll

▸ **unbindAll**(): `void`

移除所有事件与设计器的绑定

**`代码示例`**
```
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, function(event,data){
    console.log("file has loaded")
});
designer.unbindAll();
```

#### Returns

`void`

___

### <a id="registercomponent" name="registercomponent"></a> RegisterComponent

▸ `Static` **RegisterComponent**(`name`, `constructor`): `boolean`

注册自定义组件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 组件名称，用此名称使用组件 |
| `constructor` | `any` | 组件类 |

#### Returns

`boolean`

是否注册成功
