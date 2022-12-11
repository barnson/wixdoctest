---
custom_edit_url: null
sidebar_position: 16
---
# Font element (Thmutil extension)
Defines a font including the size and color.

## Parents
[Theme](theme.md)

## Attributes
**Background** ([FontColorType](fontcolortype.md 'Indicates the foreground or background color of a font.'))
  : A system color id or a hexadecimal value representing BGR background color of the font. "ffffff" is white, "ff0000" is pure blue, "00ff00" is pure green, "0000ff" is pure red, and "000000" is black. If this attribute is absent the background will be transparent. Supported system color ids are: btnface, btntext, graytext, highlight, highlighttext, hotlight, window, and windowtext.

**Foreground** ([FontColorType](fontcolortype.md 'Indicates the foreground or background color of a font.'))
  : A system color id or a hexadecimal value representing BGR foreground color of the font. "ffffff" is white, "ff0000" is pure blue, "00ff00" is pure green, "0000ff" is pure red, and "000000" is black. If this attribute is absent the foreground will be transparent. Supported system color ids are: btnface, btntext, graytext, highlight, highlighttext, hotlight, window, and windowtext.

**Height** (xs:int, required)
  : Font size. Use negative numbers to specify the font in pixels.

**Id** (String, required)
  : Identifier for the font.

**Underline** (enumeration)
  : Specifies whether the font is underlined. This attribute's value must be one of the following:
- *no*
- *yes*

**Weight** (xs:nonNegativeInteger)
  : Font weight.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)