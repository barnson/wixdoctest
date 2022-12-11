---
custom_edit_url: null
sidebar_position: 23
---
# Label element (Thmutil extension)
Defines a label.

## Children
* [Text](text.md) 
* [Tooltip](tooltip.md) 

## Attributes
**Center** (enumeration)
  : Specifies whether the text should be centered horizontally in the width of the control. Default is "no". This attribute's value must be one of the following:
- *no*
- *yes*

**DisablePrefix** (enumeration)
  : By default ampersands (&) in the text will underline the next character and treat it as an accelerator key. Set this attribute to "yes" to disable that behavior. Default is "no". This attribute's value must be one of the following:
- *no*
- *yes*

**EnableCondition** (String)
  : A condition that determines if the control is enabled.  If this condition is true or omitted, then the control will be enabled.

**FontId** (String)
  : Numeric identifier to the Font element that serves as the font for the control.

**Height** (xs:int, required)
  : Height of the control. Non-positive values extend the control to the bottom of the window minus the value. A zero value extends the control to the bottom of the window.

**HexStyle** (xs:hexBinary)
  : Hexadecimal window style for the control.

**HideWhenDisabled** (enumeration)
  : Specifies whether the control should be hidden when disabled. This attribute's value must be one of the following:
- *no*
- *yes*

**Name** (String)
  : Optional name for the control.

**StringId** (xs:nonNegativeInteger)
  : Identifier that references a string resource in the module to define the text for the label.

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