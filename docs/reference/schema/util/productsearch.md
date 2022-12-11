---
custom_edit_url: null
sidebar_position: 26
---
# ProductSearch element (Util extension)
Describes a product search.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**Guid** (String)
  : The Guid attribute has been deprecated; use the ProductCode or UpgradeCode attribute instead. If this attribute is used, it is assumed to be a ProductCode.

**Id** (String)
  : Id of the search for ordering and dependency.

**ProductCode** (String)
  : The ProductCode to use for the search. This attribute must be omitted if UpgradeCode is specified.

**Result** (enumeration)
  : Rather than saving the product version into the variable, a ProductSearch can save another attribute of the matching product instead. This attribute's value must be one of the following:
- *assignment*: Saves the assignment type of the product: per-user (0), or per-machine (1).
- *language*: Saves the language of a matching product if found; empty otherwise.
- *state*: Saves the state of the product: advertised (1), absent (2), or locally installed (5).
- *version*: Saves the version of a matching product if found; 0.0.0.0 otherwise. This is the default.

**UpgradeCode** (String)
  : The UpgradeCode to use for the search. This attribute must be omitted if ProductCode is specified. Note that if multiple products are found, the highest versioned product will be used for the result.

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)