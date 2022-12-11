---
custom_edit_url: null
sidebar_position: 78
---
# EmbeddedUIResource element
Defines a resource for use by the embedded UI.

## Windows Installer references
[MsiEmbeddedUI Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiembeddedui-table)

## Parents
[EmbeddedUI](embeddedui.md)

## Attributes
**Id** (String, required)
  : Identifier for the embedded UI resource.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'), required)
  : The name for the resource when it is extracted from the MSI package for use by the embedded UI DLL. (Windows Installer does not support the typical short filename and long filename combination for embedded UI files as it does for other kinds of files.) If this attribute is not specified the Id attribute will be used.

**SourceFile** (String, required)
  : Path to the binary file that is the embedded UI resource.


## See also
[EmbeddedUI](embeddedui.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)