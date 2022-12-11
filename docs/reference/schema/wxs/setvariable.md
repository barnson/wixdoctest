---
custom_edit_url: null
sidebar_position: 245
---
# SetVariable element
Schedules a "search" that sets a variable to the given value.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**Id** (String)
  : Id of the search for ordering and dependency.

**Type** (enumeration)
  : Type of the variable, inferred from the value if not specified. This attribute's value must be one of the following:
- *string*: A literal string.
- *formatted*: A string that may contain Variables.
- *numeric*
- *version*

**Value** (String)
  : New value for the variable. This string gets formatted, then converted to the specified type, then assigned to the variable. Leaving Value and Type unspecified will clear the variable.

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)