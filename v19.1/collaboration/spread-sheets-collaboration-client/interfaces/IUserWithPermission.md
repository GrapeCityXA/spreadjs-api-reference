# Interface: IUserWithPermission

表示一个带有相关权限设置的用户。
在 IUser 基础上扩展了文档权限信息。

## Hierarchy

- [`IUser`](IUser.md)

  ↳ **`IUserWithPermission`**

## Table of contents

### Properties

- [avatar](IUserWithPermission.md#avatar)
- [color](IUserWithPermission.md#color)
- [email](IUserWithPermission.md#email)
- [id](IUserWithPermission.md#id)
- [name](IUserWithPermission.md#name)
- [permission](IUserWithPermission.md#permission)

## Properties

### <a id="avatar" name="avatar"></a> avatar

• `Optional` **avatar**: [`IImageSource`](../README.md#iimagesource)

#### Inherited from

[IUser](IUser.md).[avatar](IUser.md#avatar)

___

### <a id="color" name="color"></a> color

• `Optional` **color**: `string`

#### Inherited from

[IUser](IUser.md).[color](IUser.md#color)

___

### <a id="email" name="email"></a> email

• `Optional` **email**: `string`

#### Inherited from

[IUser](IUser.md).[email](IUser.md#email)

___

### <a id="id" name="id"></a> id

• **id**: `string`

#### Inherited from

[IUser](IUser.md).[id](IUser.md#id)

___

### <a id="name" name="name"></a> name

• **name**: `string`

#### Inherited from

[IUser](IUser.md).[name](IUser.md#name)

___

### <a id="permission" name="permission"></a> permission

• `Optional` **permission**: [`IPermission`](IPermission.md)
