---
custom_edit_url: null
sidebar_position: 5
---
# ComponentSearch element (Util extension)
Describes a component search.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**Guid** (String, required)
  : Component to search for.

**Id** (String)
  : Id of the search for ordering and dependency.

**ProductCode** (String)
  : Optional ProductCode to determine if the component is installed.

**Result** (enumeration)
  : Rather than saving the matching key path into the variable, a ComponentSearch can save an attribute of the component instead. This attribute's value must be one of the following:
- *directory*: Saves the parent directory for the component's file key path; other types of key path are returned unmodified.
- *keyPath*: Saves the key path of the component if installed. This is the default.
- *state*: Saves the state of the component: absent (2), locally installed (3), will run from source (4), or installed in default location (either local or from source) (5)

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)