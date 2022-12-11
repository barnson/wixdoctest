---
custom_edit_url: null
sidebar_position: 209
---
# RemoteBundle element
Describes information about the referenced Bundle.

## Parents
[BundlePackagePayload](bundlepackagepayload.md)

## Children
* [RemoteRelatedBundle](remoterelatedbundle.md) 

## Attributes
**BundleId** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : The id of the bundle.

**DisplayName** (String)
  : The display name of the bundle.

**EngineVersion** (String)
  : The version of the bundle's engine.

**InstallSize** (String)
  : The size this bundle will take on disk in bytes after it is installed.

**ManifestNamespace** (String, required)
  : The namespace of the bundle's manifest.

**PerMachine** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'), required)
  : Whether the bundle is per-machine.

**ProviderKey** (String, required)
  : The provider key of the bundle.

**UpgradeCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : An upgrade code of the bundle.

**Version** (String, required)
  : The version of the bundle.

**Win64** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'), required)
  : Whether the bundle is 64-bit.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)