---
custom_edit_url: null
sidebar_position: 143
---
# MsiPackagePayload element
Describes information about the MsiPackage payload. Cannot be specified if the owning MsiPackage specified any of SourceFile, Name, DownloadUrl, or Compressed.

## Parents
[MsiPackage](msipackage.md), [PayloadGroup](payloadgroup.md)

## Attributes
**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Whether the package payload should be embedded in a container or left as an external payload.

**DownloadUrl** (String)
  : The URL to use to download the package. The following substitutions are supported:  {0} is replaced by the package Id. {1} is replaced by the payload Id. {2} is replaced by the payload file name.

**Id** (String)
  : The identifier of the package payload element.

**Name** (String)
  : The destination path and file name for this chain payload. Use this attribute to rename the chain entry point or extract it into a subfolder. The default value is the file name from the SourceFile attribute. At a minimum, the Name or SourceFile attribute must be specified. This must be a relative path ('\foo' or 'C:\foo' is not allowed).

**SourceFile** (String)
  : Location of the package to add to the bundle. The default value is the Name attribute, if provided. At a minimum, the SourceFile or Name attribute must be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)