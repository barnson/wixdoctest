---
custom_edit_url: null
sidebar_position: 19
---
# Image element (Thmutil extension)
Defines an image which can be shared between multiple controls. If alternates are provided, the dimensions of the destination rectangle are compared to all of the available sources: 1. If there is an exact match for width and height then that source will be used (no scaling required). 2. If there is not an exact match then the smallest source whose width and height are larger or equal to the destination will be used and downscaled. 3. If there is still no match then the largest source will be used and upscaled.

## Parents
[Theme](theme.md)

## Children
* [AlternateResolution](alternateresolution.md) 

## Attributes
**Id** (String, required)
  : Identifier for the Image.

**ImageFile** (String)
  : Relative path to an image file for the control. Mutually exclusive with ImageResource attribute.

**ImageResource** (xs:nonNegativeInteger)
  : Identifier that references an image resource with type RT_RCDATA in the module for the control. Mutually exclusive with ImageFile attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)