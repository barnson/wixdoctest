---
custom_edit_url: null
sidebar_position: 287
---
# Variable element
Describes a burn engine variable to define.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Attributes
**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether the value of the variable should be hidden.

**Name** (String, required)
  : The name for the variable.

**Persisted** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether the variable should be persisted.

**Type** (enumeration)
  : Type of the variable, inferred from the value if not specified. This attribute's value must be one of the following:
- *string*: A literal string.
- *formatted*: A string that may contain Variables.
- *numeric*
- *version*

**Value** (String)
  : Starting value for the variable.

**Overridable** (wxs:YesNoTypeUnion)
  : When set to "yes", lets the user override the variable's default value by specifying another value on the command line, in the form Variable=Value. Otherwise, WixStdBA won't overwrite the default value and will log "Ignoring attempt to set non-overridable variable: 'BAR'."


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)