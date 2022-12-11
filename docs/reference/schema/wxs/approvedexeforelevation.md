---
custom_edit_url: null
sidebar_position: 8
---
# ApprovedExeForElevation element
Provides information about an .exe so that the BA can request the engine to run it elevated from any secure location.

## Parents
[Bundle](bundle.md)

## Attributes
**Bitness** ([BitnessTypeUnion](bitnesstype.md 'Values of this type will be "default", "always32" or "always64".'))
  : Overrides the default registry to search. The value `always64` will force the search to look in the 64-bit registry even when building for 32-bit. Simliarly, the value `always32` will force the search to look in the 32-bit registry even when building for 64-bit. The default value is `default` where the search will look in the same registry as the bitness of the package.

**Id** (String, required)
  : The identifier of the ApprovedExeForElevation element.

**Key** (String, required)
  : The key path. For security purposes, the root key will be HKLM and Variables are not supported.

**Value** (String)
  : The value name. For security purposes, Variables are not supported.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)