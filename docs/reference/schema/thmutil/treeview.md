---
custom_edit_url: null
sidebar_position: 39
---
# TreeView element (Thmutil extension)
Defines a treeview.

## Attributes
**AlwaysShowSelect** ()
  : Specifies whether the row always appears selected even when the treeview has lost focus.

**EnableCondition** (String)
  : A condition that determines if the control is enabled.  If this condition is true or omitted, then the control will be enabled.

**EnableDragDrop** ()
  : Specifies whether drag and drop is enabled for the treeview.

**FullRowSelect** ()
  : Specifies whether an entire row is selected for the treeview.

**HasButtons** ()
  : Specifies whether the treeview will show buttons.

**HasLines** ()
  : Specifies whether lines appear for all treeview items.

**Height** (xs:int, required)
  : Height of the control. Non-positive values extend the control to the bottom of the window minus the value. A zero value extends the control to the bottom of the window.

**HexStyle** (xs:hexBinary)
  : Hexadecimal window style for the control.

**HideWhenDisabled** (enumeration)
  : Specifies whether the control should be hidden when disabled. This attribute's value must be one of the following:
- *no*
- *yes*

**LinesAtRoot** ()
  : Specifies whether the root nodes have lines beside them.

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