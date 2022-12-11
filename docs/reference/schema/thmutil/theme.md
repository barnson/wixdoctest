---
custom_edit_url: null
sidebar_position: 37
---
# Theme element (Thmutil extension)
This is the top-level container element for every thmutil Theme file.

## Children
* [Font](font.md) 
* [Image](image.md) 
* [ImageList](imagelist.md) 
* [Window](window.md) 

## Attributes
**ImageFile** (String)
  : Relative path to an image file that can serve as a single source for images in the rest of the theme. This image is referenced by controls using the SourceX and SourceY attributes. Mutually exclusive with the ImageResource attribute.

**ImageResource** (String)
  : Identifier that references an image resource in the module for the window. This image is referenced by controls using the SourceX and SourceY attributes. Mutually exclusive with the ImageFile attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)