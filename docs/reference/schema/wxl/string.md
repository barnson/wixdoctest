---
custom_edit_url: null
sidebar_position: 1
---
# String element (Wxl extension)


## Parents
[WixLocalization](wixlocalization.md)

## Attributes
**Id** (String, required)
  : Identity of the localized string. Referenced in .wxs files using `!(loc.Id)` or in locutil using `#(loc.Id)`.

**Localizable** (enumeration)
  : Indicates whether the string is localizable text or a non-localizable string that must be unique per locale. The value of this attribute is not used by the WiX Toolset. It provided as documentation for localizers to ignore things like GUIDs or identifiers that look like text. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**Overridable** (enumeration)
  : Determines if the localized string may be overridden by a definition in another localization file. The default value is `no`. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**Value** (String)
  : The localized value for this string.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wixloc.xsd)