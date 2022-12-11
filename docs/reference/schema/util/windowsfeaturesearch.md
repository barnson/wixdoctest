---
custom_edit_url: null
sidebar_position: 41
---
# WindowsFeatureSearch element (Util extension)
Detects the existence of a Windows feature.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**Feature** (enumeration, required)
  : The feature to detect. This attribute's value must be one of the following:
- *sha2CodeSigning*: The oldest OS with this feature is Win7 SP1 with KB3033929.

**Id** (String)
  : Id of the search for ordering and dependency.

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)