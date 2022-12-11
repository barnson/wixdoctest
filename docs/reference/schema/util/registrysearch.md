---
custom_edit_url: null
sidebar_position: 32
---
# RegistrySearch element (Util extension)
Describes a registry search.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Bitness** (wxs:BitnessTypeUnion)
  : Overrides the default registry to search. The value `always64` will force the search to look in the 64-bit registry even when building for 32-bit. Simliarly, the value `always32` will force the search to look in the 32-bit registry even when building for 64-bit. The default value is `default` where the search will look in the same registry as the bitness of the package.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**ExpandEnvironmentVariables** (wxs:YesNoTypeUnion)
  : Whether to expand any environment variables in REG_SZ, REG_EXPAND_SZ, or REG_MULTI_SZ values.

**Id** (String)
  : Id of the search for ordering and dependency.

**Key** (String, required)
  : Key to search for.

**Result** (enumeration)
  : Rather than saving the matching registry value into the variable, a RegistrySearch can save an attribute of the matching entry instead. This attribute's value must be one of the following:
- *exists*: Saves true if a matching registry entry is found; false otherwise.
- *value*: Saves the value of the registry key in the variable. This is the default.

**Root** (enumeration, required)
  : Registry root hive to search under. This attribute's value must be one of the following:
- *HKLM*: HKEY_LOCAL_MACHINE
- *HKCU*: HKEY_CURRENT_USER
- *HKCR*: HKEY_CLASSES_ROOT
- *HKU*: HKEY_USERS

**Value** (String)
  : Optional value to search for under the given Key.

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)