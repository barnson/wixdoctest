---
custom_edit_url: null
sidebar_position: 82
---
# Exclusion element
Declares a merge module with which this merge module is incompatible.

## Parents
[Module](module.md)

## Attributes
**ExcludedId** (String, required)
  : Identifier of the merge module that is incompatible.

**ExcludedMaxVersion** (String)
  : Maximum version excluded from a range. If not set, all versions after min are excluded. If neither max nor min, no exclusion based on version.

**ExcludedMinVersion** (String)
  : Minimum version excluded from a range. If not set, all versions before max are excluded. If neither max nor min, no exclusion based on version.

**ExcludeExceptLanguage** (Integer)
  : Numeric language ID of the merge module in ExcludedID. All except this language will be excluded. Only one of ExcludeExceptLanguage and ExcludeLanguage may be specified.

**ExcludeLanguage** (Integer)
  : Numeric language ID of the merge module in ExcludedID. The specified language will be excluded. Only one of ExcludeExceptLanguage and ExcludeLanguage may be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)