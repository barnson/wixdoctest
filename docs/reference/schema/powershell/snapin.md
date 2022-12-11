---
custom_edit_url: null
sidebar_position: 2
---
# SnapIn element (Powershell extension)
Identifies the parent File as a PowerShell snap-in to be registered on the system.

## Parents
[File](../wxs/file.md)

## Children
* [FormatsFile](formatsfile.md) 
* [TypesFile](typesfile.md) 

## Remarks
[PowerShell](http://www.microsoft.com/powershell) snap-ins allow developers to
extend the functionality of of the PowerShell engine. Add this element to identify
the parent File as a PowerShell snap-in that will get registered on the system.


## Attributes
**CustomSnapInType** (String)
  : The full type name of a class that is used to register a list of cmdlets and providers.

**Description** (String)
  : A brief description of the snap-in.

**DescriptionIndirect** ([EmbeddedResource](embeddedresource.md 'Values should be in the format *ResourceName,StringName*, where *ResourceName* is the name of the embedded resource in your assembly sans the ".resources" extension, and *StringName* is the name of the string resource in the embedded resource.   Example: UtilityMshSnapInResources,Description'))
  : An embedded resource that contains a brief description of the snap-in. This resource must be embedded in the current snap-in assembly.

**Id** (String, required)
  : The identifier for this PowerShell snap-in.

**RequiredPowerShellVersion** (wxs:VersionType)
  : The required version of PowerShell that must be installed and is associated with the snap-in registration. The default value is "1.0".

**Vendor** (String)
  : The name of the snap-in vendor.

**VendorIndirect** ([EmbeddedResource](embeddedresource.md 'Values should be in the format *ResourceName,StringName*, where *ResourceName* is the name of the embedded resource in your assembly sans the ".resources" extension, and *StringName* is the name of the string resource in the embedded resource.   Example: UtilityMshSnapInResources,Description'))
  : An embedded resource that contains the name of the snap-in vendor. This resource must be embedded in the current snap-in assembly.

**Version** (wxs:VersionType)
  : The version of the snapin. If not specified, this is taken from the assembly name.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/ps.xsd)