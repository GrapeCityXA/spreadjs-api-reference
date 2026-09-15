# Class: Server

协作服务器，提供双向通信、中间件和钩子机制。

## Table of contents

### Constructors

- [constructor](Server.md#constructor)

### Methods

- [on](Server.md#on)
- [use](Server.md#use)
- [useFeature](Server.md#usefeature)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Server**(`config?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config?` | [`IServerConfig`](../interfaces/IServerConfig.md) |

## Methods

### <a id="on" name="on"></a> on

▸ **on**(`hooks`): `void`

向服务器注册钩子

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hooks` | [`IHooks`](../interfaces/IHooks.md) | 要注册的钩子 |

#### Returns

`void`

▸ **on**<`K`\>(`action`, `hook`): `void`

向服务器注册钩子

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends keyof [`IHookContext`](../interfaces/IHookContext.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | `K` | 动作名称 |
| `hook` | [`IHook`](../interfaces/IHook.md)<[`IHookContext`](../interfaces/IHookContext.md)[`K`]\> | 要注册的钩子 |

#### Returns

`void`

___

### <a id="use" name="use"></a> use

▸ **use**(`middlewares`): `void`

向服务器注册中间件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `middlewares` | [`IMiddlewares`](../interfaces/IMiddlewares.md) | 要注册的中间件 |

#### Returns

`void`

▸ **use**<`K`\>(`action`, `middleware`): `void`

向服务器注册中间件

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends keyof [`IMiddlewareContext`](../interfaces/IMiddlewareContext.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | `K` | 动作名称 |
| `middleware` | [`IMiddleware`](../interfaces/IMiddleware.md)<[`IMiddlewareContext`](../interfaces/IMiddlewareContext.md)[`K`]\> | 要注册的中间件 |

#### Returns

`void`

___

### <a id="usefeature" name="usefeature"></a> useFeature

▸ **useFeature**(`feature`): `void`

向服务器注册功能

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `feature` | [`IFeature`](../interfaces/IFeature.md) | 要注册的功能 |

#### Returns

`void`
