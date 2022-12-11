---
custom_edit_url: null
sidebar_position: 40
---
# Window element (Thmutil extension)
Defines the overall look of the main window.

## Parents
[Theme](theme.md)

## Children
* [Page](page.md) 

## Attributes
**AutoResize** (enumeration)
  : Specifies whether the ThmUtil default window proc should process WM_SIZE and WM_SIZING events. This attribute's value must be one of the following:
- *no*
- *yes*

**Caption** (String)
  : Caption for the window. This is required if not using the StringId attribute.

**FontId** (String, required)
  : Identifier to the Font element that serves as the default font for the window.

**Height** (xs:positiveInteger, required)
  : Height of the window's client area.

**HexStyle** (xs:hexBinary)
  : Hexadecimal window style. If this is not specified the default value is: WS_OVERLAPPED | WS_VISIBLE | WS_MINIMIZEBOX | WS_SYSMENU | WS_CAPTION. If SourceX and SourceY are specified, then WS_OVERLAPPED is replaced with WS_POPUP.

**IconFile** (String)
  : Relative path to an icon file for the window. Mutually exclusive with IconResource attribute.

**IconResource** (String)
  : Identifier that references an icon resource in the module for the icon for the window. Mutually exclusive with IconFile attribute.

**MinimumHeight** (xs:positiveInteger)
  : Minimum height of the window. Can only be specified if AutoResize is enabled.

**MinimumWidth** (xs:positiveInteger)
  : Minimum width of the window. Can only be specified if AutoResize is enabled.

**SourceX** (xs:nonNegativeInteger)
  : X offset of the window background in the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource.

**SourceY** (xs:nonNegativeInteger)
  : Y offset of the window background in the Theme/@ImageFile or Theme/@ImageResource. Can only be specified with Theme/@ImageFile or Theme/@ImageResource.

**StringId** (xs:nonNegativeInteger)
  : Identifier that references a string resource in the module to define the window caption. Mutually exclusive with the Caption attribute.

**Width** (xs:positiveInteger, required)
  : Width of the window's client area.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)