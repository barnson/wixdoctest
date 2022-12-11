---
custom_edit_url: null
sidebar_position: 6
---
# ButtonHoverImage element (Thmutil extension)
Defines a button image that is used when the control is hovered over. ButtonImage and ButtonSelectedImage are required with ButtonHoverImage.

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