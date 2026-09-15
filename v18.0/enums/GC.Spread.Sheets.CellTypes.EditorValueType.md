# Enumeration: EditorValueType

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).EditorValueType

 指定从中写入所选项的数据模型的内容
 提供多种值选择的某些单元格类型

**`readonly`**

**`代码示例`**
``` javascript
//本示例使用EditorValueType枚举
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a","b","c"]);
cellType2.editorValueType(GC.Spread.Sheets.CellTypes.EditorValueType.text);
activeSheet.getCell(2, 2).cellType(cellType2);
```

## Table of contents

### Enumeration members

- [index](GC.Spread.Sheets.CellTypes.EditorValueType.md#index)
- [text](GC.Spread.Sheets.CellTypes.EditorValueType.md#text)
- [value](GC.Spread.Sheets.CellTypes.EditorValueType.md#value)

## Enumeration members

### <a id="index" name="index"></a> index

• **index** = `1`

将所选项的索引写入模型

___

### <a id="text" name="text"></a> text

• **text** = `0`

 将所选项的文本值写入模型

___

### <a id="value" name="value"></a> value

• **value** = `2`

 将所选项的相应数据值写入模型
