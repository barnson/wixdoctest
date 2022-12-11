---
custom_edit_url: null
sidebar_position: 1
---
# DotNetCompatibilityCheck element (Netfx extension)
Validates whether the specified .NET is installed on the computer.

## Parents
[Package](../wxs/package.md), [Module](../wxs/module.md)

## Attributes
**Id** (String)
  : Identifier for the compatibility check. If the Id is not specified, one will be generated.

**Platform** (enumeration)
  : The platform to use to validate. This attribute's value must be one of the following:
- *arm64*
- *x64*
- *x86*

**Property** (String, required)
  : Name of the property in which to place the result of the compatibility check. The possible values are:  0 - Successful compatibility check. 1 - No runtime is installed. 2 - Required runtime is not installed. 3 - Failed to get hostfxr exports. 4 - Invalid arguments. 5 - Failed to construct temp json file path. 6 - Failed to create temp json file.

**RollForward** (enumeration)
  : The roll forward policy to use while validating. This attribute's value must be one of the following:
- *latestMajor*
- *major*
- *latestMinor*
- *minor*
- *latestPatch*
- *disable*

**RuntimeType** (enumeration)
  : The .NET runtime to check against. This attribute's value must be one of the following:
- *aspnet*
- *core*
- *desktop*

**Version** (wxs:VersionType)
  : Version of .NET to check against.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/netfx.xsd)