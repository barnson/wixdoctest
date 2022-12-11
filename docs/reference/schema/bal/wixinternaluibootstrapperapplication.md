---
custom_edit_url: null
sidebar_position: 4
---
# WixInternalUIBootstrapperApplication element (Bal extension)
Uses WixInternalUIBootstrapperApplication as the Bootstrapper Application for a Bundle. WixInternalUIBootstrapperApplication has no UI itself, it relies on the splash screen, prereq BA, and MSI UI.  wixiuiba is not a typical BA because it has very specific requirements for the packages in the chain. There can only be one non-permanent package in the chain, and it needs to be the last package. The only exception is that multiple non-permanent packages can be specified with bal:PrimaryPackageType with a specific architecture. Each primary package must be an MsiPackage that contains UI for install and maintenance.  If there are permanent packages, then they are always installed through the same prereq BA that is used for the managed BA hosts before executing the primary package.  Due to Windows limitations, a splash screen should be provided so that the elevation prompt and MSI UI is automatically given focus.

## Parents
[BootstrapperApplication](../wxs/bootstrapperapplication.md)

## Attributes
**LocalizationFile** (String)
  : Source file of the theme localization .wxl file.

**LogoFile** (String)
  : Source file of the logo graphic.

**Theme** (enumeration)
  : The built-in theme to use. This attribute's value must be one of the following:
- *none*
- *standard*

**ThemeFile** (String)
  : Source file of the theme XML.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/bal.xsd)