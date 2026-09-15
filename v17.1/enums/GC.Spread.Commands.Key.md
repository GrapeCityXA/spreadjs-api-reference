# Enumeration: Key

[Spread](../modules/GC.Spread.md).[Commands](../modules/GC.Spread.Commands.md).Key

按键编码

**`代码示例`**
```
//本示例使用回车键创建一个自定义操作
var activeSheet = spread.getActiveSheet();
spread.commandManager().register('myCmd',
                function ColorAction() {
                    //单击一个单元格，然后按Enter键
                    activeSheet.getCell(activeSheet.getActiveRowIndex(), activeSheet.getActiveColumnIndex()).backColor("red");
                }
            );
//将创建的操作映射到回车键
spread.commandManager().setShortcutKey('myCmd', GC.Spread.Commands.Key.enter, false, false, false, false);
```

## Table of contents

### Enumeration members

- [a](GC.Spread.Commands.Key.md#a)
- [altkey](GC.Spread.Commands.Key.md#altkey)
- [backspace](GC.Spread.Commands.Key.md#backspace)
- [c](GC.Spread.Commands.Key.md#c)
- [ctrl](GC.Spread.Commands.Key.md#ctrl)
- [del](GC.Spread.Commands.Key.md#del)
- [down](GC.Spread.Commands.Key.md#down)
- [end](GC.Spread.Commands.Key.md#end)
- [enter](GC.Spread.Commands.Key.md#enter)
- [esc](GC.Spread.Commands.Key.md#esc)
- [home](GC.Spread.Commands.Key.md#home)
- [left](GC.Spread.Commands.Key.md#left)
- [pdn](GC.Spread.Commands.Key.md#pdn)
- [pup](GC.Spread.Commands.Key.md#pup)
- [right](GC.Spread.Commands.Key.md#right)
- [shift](GC.Spread.Commands.Key.md#shift)
- [space](GC.Spread.Commands.Key.md#space)
- [tab](GC.Spread.Commands.Key.md#tab)
- [up](GC.Spread.Commands.Key.md#up)
- [v](GC.Spread.Commands.Key.md#v)
- [x](GC.Spread.Commands.Key.md#x)
- [y](GC.Spread.Commands.Key.md#y)
- [z](GC.Spread.Commands.Key.md#z)

## Enumeration members

### <a id="a" name="a"></a> a

• **a** = `65`

A键

___

### <a id="altkey" name="altkey"></a> altkey

• **altkey** = `18`

Alt键

___

### <a id="backspace" name="backspace"></a> backspace

• **backspace** = `8`

退格键

___

### <a id="c" name="c"></a> c

• **c** = `67`

C键

___

### <a id="ctrl" name="ctrl"></a> ctrl

• **ctrl** = `17`

Ctrl键

___

### <a id="del" name="del"></a> del

• **del** = `46`

删除键

___

### <a id="down" name="down"></a> down

• **down** = `40`

向下箭头键

___

### <a id="end" name="end"></a> end

• **end** = `35`

End键

___

### <a id="enter" name="enter"></a> enter

• **enter** = `13`

回车键

___

### <a id="esc" name="esc"></a> esc

• **esc** = `27`

Esc键

___

### <a id="home" name="home"></a> home

• **home** = `36`

Home键

___

### <a id="left" name="left"></a> left

• **left** = `37`

左箭头键

___

### <a id="pdn" name="pdn"></a> pdn

• **pdn** = `34`

Page Down键

___

### <a id="pup" name="pup"></a> pup

• **pup** = `33`

Page Up键

___

### <a id="right" name="right"></a> right

• **right** = `39`

右箭头键

___

### <a id="shift" name="shift"></a> shift

• **shift** = `16`

Shift键

___

### <a id="space" name="space"></a> space

• **space** = `32`

空格键

___

### <a id="tab" name="tab"></a> tab

• **tab** = `9`

Tab键

___

### <a id="up" name="up"></a> up

• **up** = `38`

向上箭头键

___

### <a id="v" name="v"></a> v

• **v** = `86`

V键

___

### <a id="x" name="x"></a> x

• **x** = `88`

X键

___

### <a id="y" name="y"></a> y

• **y** = `89`

Y键

___

### <a id="z" name="z"></a> z

• **z** = `90`

Z键
