# js-collaboration-presence

## Table of contents

### Functions

- [presenceFeature](README.md#presencefeature)

## Functions

### <a id="presencefeature" name="presencefeature"></a> presenceFeature

▸ **presenceFeature**(): `IFeature`

在线状态功能

**`example`**
const httpServer = createServer();
const server = new Server({ httpServer });
server.useFeature(OT.documentFeature());
server.useFeature(presenceFeature());

#### Returns

`IFeature`
