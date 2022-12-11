---
custom_edit_url: null
sidebar_position: 24
---
# ListView element (Thmutil extension)
Defines a listview.

## Children
* [Column](column.md) 

## Attributes
**EnableCondition** (String)
  : A condition that determines if the control is enabled.  If this condition is true or omitted, then the control will be enabled.

**FontId** (String)
  : Identifier to the Font element that serves as the default font for the ListView.

**Height** (xs:int, required)
  : Height of the control. Non-positive values extend the control to the bottom of the window minus the value. A zero value extends the control to the bottom of the window.

**HexExtendedStyle** (xs:hexBinary)
  : Hexadecimal extended window style.

**HexStyle** (xs:hexBinary)
  : Hexadecimal window style for the control.

**HideWhenDisabled** (enumeration)
  : Specifies whether the control should be hidden when disabled. This attribute's value must be one of the following:
- *no*
- *yes*

**ImageList** (String)
  : The name of the ImageList to assign to this listview with type LVSIL_NORMAL.

**ImageListGroupHeader** (String)
  : The name of the ImageList to assign to this listview with type LVSIL_GROUPHEADER.

**ImageListSmall** (String)
  : The name of the ImageList to assign to this listview with type LVSIL_SMALL.

**ImageListState** (String)
  : The name of the ImageList to assign to this listview with type LVSIL_STATE.

**Name** (String)
  : Optional name for the control.

**TabStop** (enumeration)
  : Specifies whether the control is part of the tab sequence of controls. This attribute's value must be one of the following:
- *no*
- *yes*

**Visible** (enumeration)
  : Specifies whether the control is initially visible. This attribute's value must be one of the following:
- *no*
- *yes*

**VisibleCondition** (String)
  : A condition that determines if the control is visible.  If this condition is true or omitted, then the control will be visible.

**Width** (xs:int, required)
  : Width of the control. Non-positive values extend the control to the right of the window minus the value. A zero value extends the control to the right of the window.

**X** (xs:int, required)
  : X coordinate for the control from the left of the window. Negative values are coordinates from the right of the window minus the width of the control.

**Y** (xs:int, required)
  : Y coordinate for the control from the top of the window. Negative values are coordinates from the bottom of the window minus the height of the control.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)