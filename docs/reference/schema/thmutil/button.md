---
custom_edit_url: null
sidebar_position: 4
---
# Button element (Thmutil extension)
Defines a button.

## Children
* [BrowseDirectoryAction](browsedirectoryaction.md) 
* [ButtonFocusImage](buttonfocusimage.md) 
* [ButtonHoverImage](buttonhoverimage.md) 
* [ButtonImage](buttonimage.md) 
* [ButtonSelectedImage](buttonselectedimage.md) 
* [ChangePageAction](changepageaction.md) 
* [CloseWindowAction](closewindowaction.md) 
* [Text](text.md) 
* [Tooltip](tooltip.md) 

## Attributes
**EnableCondition** (String)
  : A condition that determines if the control is enabled.  If this condition is true or omitted, then the control will be enabled.

**FontId** (String)
  : Identifier to the Font element that serves as the font for the control. Only valid when using graphic buttons.

**Height** (xs:int, required)
  : Height of the control. Non-positive values extend the control to the bottom of the window minus the value. A zero value extends the control to the bottom of the window.

**HexStyle** (xs:hexBinary)
  : Hexadecimal window style for the control.

**HideWhenDisabled** (enumeration)
  : Specifies whether the control should be hidden when disabled. This attribute's value must be one of the following:
- *no*
- *yes*

**HoverFontId** (String)
  : Identifier to the Font element that serves as the font when the control is hovered over. Only valid when using graphic buttons.

**ImageFile** (String)
  : Relative path to an image file for the control. Mutually exclusive with ImageId and ImageResource and SourceX and SourceY attributes.

**ImageId** (String)
  : Identifier to the Image element that serves as the image for the control. Mutually exclusive with ImageFile and ImageResource and SourceX and SourceY attributes.

**ImageResource** (xs:nonNegativeInteger)
  : Identifier that references an image resource with type RT_RCDATA in the module for the control. Mutually exclusive with ImageId and ImageFile and SourceX and SourceY attributes.

**Name** (String)
  : Optional name for the control.

**SelectedFontId** (String)
  : Identifier to the Font element that serves as the font when the control is selected. Only valid when using graphic buttons.

**SourceX** (xs:nonNegativeInteger)
  : X offset of the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource. Mutually exclusive with ImageId and ImageFile and ImageResource attributes.

**SourceY** (xs:nonNegativeInteger)
  : Y offset of the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource. Mutually exclusive with ImageId and ImageFile and ImageResource attributes.

**StringId** (xs:nonNegativeInteger)
  : Identifier that references a string resource in the module to define the text for the control.

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