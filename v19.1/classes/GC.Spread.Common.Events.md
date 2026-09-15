# Class: Events

[Spread](../modules/GC.Spread.md).[Common](../modules/GC.Spread.Common.md).Events

## Table of contents

### Constructors

- [constructor](GC.Spread.Common.Events.md#constructor)

### Events

- [CurrentUserChanged](GC.Spread.Common.Events.md#currentuserchanged)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Events**()

定义UserManager支持的事件。

## Events

### <a id="currentuserchanged" name="currentuserchanged"></a> CurrentUserChanged

• `Static` **CurrentUserChanged**: `string`

指示当前用户发生更改时的事件。

**`param`** *{@link GC.Spread.Common.IUser}* `oldCurrentUser` 旧的当前用户。

**`param`** *{@link GC.Spread.Common.IUser}* `newCurrentUser` 新的当前用户。

**`example`**
```javascript
GC.Spread.Common.UserManager.bind(GC.Spread.Common.Events.CurrentUserChanged, (event, args) => {
    console.log(event);
    console.log(args.oldCurrentUser);
    console.log(args.newCurrentUser);
});
```
