---
custom_edit_url: null
sidebar_position: 55
---
# Custom element
Use to sequence a custom action.

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md), [AdminUISequence](adminuisequence.md), [AdminExecuteSequence](adminexecutesequence.md), [AdvertiseExecuteSequence](advertiseexecutesequence.md)

## Attributes
**Action** (String, required)
  : The CustomAction to which the Custom element applies.

**After** (String)
  : The name of the standard or custom action after which this action should be performed. Mutually exclusive with Before, OnExit, and Sequence attributes

**Before** (String)
  : The name of the standard or custom action before which this action should be performed. Mutually exclusive with OnExit, After, and Sequence attributes

**Condition** (String)
  : Optional condition that determines whether the action should be executed.

**OnExit** (enumeration)
  : Mutually exclusive with Before, After, and Sequence attributes This attribute's value must be one of the following:
- *success*
- *cancel*
- *error*
- *suspend*

**Overridable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If "yes", the sequencing of this action may be overridden by sequencing elsewhere.

**Sequence** (Integer)
  : The sequence number for this action. It is recommended to use one of the other mutually exclusive attributes: OnExit, After, and Before.


## See also
[CustomAction](customaction.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)