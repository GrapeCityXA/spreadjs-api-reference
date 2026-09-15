# js-collaboration-presence

## Table of contents

### Functions

- [presenceFeature](Overview.md#presencefeature)

## Functions

### <a id="presencefeature" name="presencefeature"></a> presenceFeature

▸ **presenceFeature**(): `IFeature`

创建一个用于协作的实时功能。

**`example`**
const httpServer = createServer();
const server = new Server({ httpServer });
server.useFeature(OT.documentFeature());
server.useFeature(presenceFeature());

#### Returns

`IFeature`

实时功能。
