---
custom_edit_url: null
sidebar_position: 2
---
# UI element (Wxl extension)
Allows a localization to override the position, size, and text of dialogs and controls.

## Parents
[WixLocalization](wixlocalization.md)

## Attributes
**Control** (String)
  : Combined with the Dialog attribute, identifies the control to localize.

**Dialog** (String)
  : Identifies the dialog to localize or the dialog that a control to localize is in.

**Height** (Integer)
  : For a dialog, overrides the authored height in dialog units. For a control, overrides the authored height of the rectangular boundary of the control. This must be a non-negative number.

**LeftScroll** (enumeration)
  : Set this attribute to "yes" to cause the scroll bar to display on the left side of the Control. Not valid for a dialog. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**RightAligned** (enumeration)
  : Set this attribute to "yes" to cause the Control to be right aligned. Not valid for a dialog. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**RightToLeft** (enumeration)
  : Set this attribute to "yes" to cause the Control to display from right to left. Not valid for a dialog. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**Text** (String)
  : Override the text of a UI element.

**Width** (Integer)
  : For a dialog, overrides the authored width in dialog units. For a control, overrides the authored width of the rectangular boundary of the control. This must be a non-negative number.

**X** (Integer)
  : For a dialog, overrides the authored horizontal centering. For a control, overrides the authored horizontal coordinate of the upper-left corner of the rectangular boundary. This must be a non-negative number.

**Y** (Integer)
  : For a dialog, overrides the authored vertical centering. For a control, overrides the authored vertical coordinate of the upper-left corner of the rectangular boundary of the control. This must be a non-negative number.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wixloc.xsd)