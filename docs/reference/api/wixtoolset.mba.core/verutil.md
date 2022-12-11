---
custom_edit_url: null
toc_max_heading_level: 2
---
# VerUtil Class
Managed wrapper for verutil.
## Methods
| Method | Description |
| ------ | ----------- |
| [CompareParsedVersions()](#compareparsedversions_nop) |  |
| [CompareStringVersions()](#comparestringversions_nop) |  |
| [CopyVersion(version)](#copyversion_version) |  |
| [ParseVersion(version, strict)](#parseversion_version_strict) |  |
| [VersionFromQword(version)](#versionfromqword_version) |  |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CompareParsedVersions() Method {#compareparsedversions_nop}

### Declaration
```cs
public static int CompareParsedVersions
```
### Return value
`int` 0 if equal, 1 if version1 {'>'} version2, -1 if version1 {'<'} version2
## CompareStringVersions() Method {#comparestringversions_nop}

### Declaration
```cs
public static int CompareStringVersions
```
### Return value
`int` 0 if equal, 1 if version1 {'>'} version2, -1 if version1 {'<'} version2
## CopyVersion(version) Method {#copyversion_version}

### Declaration
```cs
public static VerUtilVersion CopyVersion(
  VerUtilVersion version
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| version | VerUtilVersion |  |
## ParseVersion(version, strict) Method {#parseversion_version_strict}

### Declaration
```cs
public static VerUtilVersion ParseVersion(
  string version,
  bool strict
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| version | string |  |
| strict | bool | Whether to throw exception on invalid version. |
## VersionFromQword(version) Method {#versionfromqword_version}

### Declaration
```cs
public static VerUtilVersion VersionFromQword(
  System.Int64 version
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| version | System.Int64 |  |
