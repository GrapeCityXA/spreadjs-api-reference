# Namespace: AI

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).AI

## Table of contents

### Type aliases

- [AIRequestCallback](GC.Spread.Sheets.AI.md#airequestcallback)
- [IAIConfig](GC.Spread.Sheets.AI.md#iaiconfig)
- [IAIEnvironment](GC.Spread.Sheets.AI.md#iaienvironment)

## Type aliases

### <a id="airequestcallback" name="airequestcallback"></a> AIRequestCallback

Ƭ **AIRequestCallback**: (`config`: [`IAIConfig`](GC.Spread.Sheets.AI.md#iaiconfig)) => `Promise`<`any`\>

#### Type declaration

▸ (`config`): `Promise`<`any`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `config` | [`IAIConfig`](GC.Spread.Sheets.AI.md#iaiconfig) |

##### Returns

`Promise`<`any`\>

___

### <a id="iaiconfig" name="iaiconfig"></a> IAIConfig

Ƭ **IAIConfig**: `Object`

**`property`** {{ role: string; content: string }[]} [messages]

**`property`** {number} [temperature]

**`property`** {number} [max_tokens]

**`property`** {boolean} [stream]

#### Index signature

▪ [key: `string`]: `any`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `max_tokens?` | `number` |
| `messages` | { `content`: `string` ; `role`: `string`  }[] |
| `stream?` | `boolean` |
| `temperature?` | `number` |

___

### <a id="iaienvironment" name="iaienvironment"></a> IAIEnvironment

Ƭ **IAIEnvironment**: `Object`

**`property`** {string} model

**`property`** {string} key

**`property`** {string} basePath

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `basePath` | `string` | 接收 JSON 请求体的 HTTP 端点，例如服务器路由或兼容 OpenAI 的 API URL。 |
| `key` | `string` | 用于 `Authorization: Bearer` 请求头中的 API 密钥。 |
| `model` | `string` | 组的所有者。 |
