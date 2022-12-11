---
custom_edit_url: null
sidebar_position: 12
---
# Column element (Thmutil extension)
A column of a list.

## Parents
[ListView](listview.md)

## Attributes
**Expands** (enumeration)
  : Whether or not this column can grow to fill available width of the listview. More than one column can be marked with yes - all expandable columns will share available extra space. This is especially useful if the Window/@AutoResize is yes. This attribute's value must be one of the following:
- *no*
- *yes*

**StringId** (xs:nonNegativeInteger)
  : Identifier that references a string resource in the module to define the text for the column header.

**Width** (xs:int)
  : Width of the column.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)