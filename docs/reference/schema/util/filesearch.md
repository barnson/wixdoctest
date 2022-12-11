---
custom_edit_url: null
sidebar_position: 13
---
# FileSearch element (Util extension)
Describes a file search.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**DisableFileRedirection** (wxs:YesNoTypeUnion)
  : When set to "yes" and the running bundle is 32-bit, Wow64DisableWow64FsRedirection is called before starting the search.

**Id** (String)
  : Id of the search for ordering and dependency.

**Path** (String)
  : File path to search for.

**Result** (enumeration)
  : Rather than saving the matching file path into the variable, a FileSearch can save an attribute of the matching file instead. This attribute's value must be one of the following:
- *exists*: Saves true if a matching file is found; false otherwise.
- *version*: Saves the version information for files that have it (.exe, .dll); zero-version (0.0.0.0) otherwise.

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)