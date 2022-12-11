---
custom_edit_url: null
sidebar_position: 251
---
# Show element


## Parents
[InstallUISequence](installuisequence.md), [AdminUISequence](adminuisequence.md)

## Attributes
**After** (String)
  : Show the dialog after the specified action. Mutually exclusive with OnExit, Before, and Sequence attributes.

**Before** (String)
  : Show the dialog before the specified action. Mutually exclusive with OnExit, After, and Sequence attributes.

**Condition** (String)
  : Optional condition that determines whether the dialog should be displayed.

**Dialog** (String, required)
  : Reference to dialog to show.

**OnExit** (enumeration)
  : Show the dialog Mutually exclusive with Before, After, and Sequence attributes. This attribute's value must be one of the following:
- *success*
- *cancel*
- *error*
- *suspend*

**Overridable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If "yes", the sequencing of this dialog may be overridden by sequencing elsewhere. The default is "no".

**Sequence** (Integer)
  : Show the dialog at the specified sequence. It is recommended to use one of the other mutually exclusive attributes: OnExit, After, and Before.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)