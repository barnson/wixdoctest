---
custom_edit_url: null
sidebar_position: 5
---
# ButtonFocusImage element (Thmutil extension)
Defines a button image that is used when the control has focus. ButtonImage, ButtonHoverImage, and ButtonSelectedImage are required with ButtonFocusImage. If not specified, then the default focus rectangle is drawn on top of ButtonImage.

## Parents
[Button](button.md)

## Attributes
**ImageFile** (String)
  : Relative path to an image file for the control. Mutually exclusive with ImageId and ImageResource and SourceX and SourceY attributes.

**ImageId** (String)
  : Identifier to the Image element that serves as the image for the control. Mutually exclusive with ImageFile and ImageResource and SourceX and SourceY attributes.

**ImageResource** (xs:nonNegativeInteger)
  : Identifier that references an image resource with type RT_RCDATA in the module for the control. Mutually exclusive with ImageId and ImageFile and SourceX and SourceY attributes.

**SourceX** (xs:nonNegativeInteger)
  : X offset of the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource. Mutually exclusive with ImageId and ImageFile and ImageResource attributes.

**SourceY** (xs:nonNegativeInteger)
  : Y offset of the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource. Mutually exclusive with ImageId and ImageFile and ImageResource attributes.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)