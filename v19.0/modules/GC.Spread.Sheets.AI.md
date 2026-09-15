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

| Name | Type |
| :------ | :------ |
| `basePath` | `string` |
| `key` | `string` |
| `model` | `string` |
