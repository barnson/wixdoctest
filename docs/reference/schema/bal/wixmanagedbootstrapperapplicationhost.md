---
custom_edit_url: null
sidebar_position: 5
---
# WixManagedBootstrapperApplicationHost element (Bal extension)
Uses WixManagedBootstrapperApplicationHost as the Bootstrapper Application for a Bundle.

## Parents
[BootstrapperApplication](../wxs/bootstrapperapplication.md)

## Attributes
**AlwaysInstallPrereqs** (String)
  : When not set or set to "no", the prereq BA is only used when the .NET Framework runtime can't be loaded. When set to "yes", the prereq BA will always run before the .NET Framework runtime is attempted to be loaded. If set to "yes" and all prereq packages are already installed, then the prereq BA's UI is not shown.

**LocalizationFile** (String)
  : Source file of the theme localization .wxl file.

**LogoFile** (String)
  : Source file of the logo graphic.

**Theme** (enumeration)
  : The built-in theme to use. The default is "standard". This attribute's value must be one of the following:
- *none*
- *standard*

**ThemeFile** (String)
  : Source file of the theme XML.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/bal.xsd)