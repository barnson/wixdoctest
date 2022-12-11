---
custom_edit_url: null
sidebar_position: 244
---
# SetProperty element
Sets a Property to a particular value. This is accomplished by creating a Type 51 custom action that is appropriately scheduled in the InstallUISequence and InstallExecuteSequence.

## Windows Installer references
[CustomAction Table](https://docs.microsoft.com/en-us/windows/win32/msi/customaction-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Attributes
**Action** (String)
  : By default the action is "Set" + Id attribute's value. This optional attribute can override the action name in the case where multiple SetProperty elements target the same Id (probably with mutually exclusive conditions).

**After** (String)
  : The name of the standard or custom action after which this action should be performed. Mutually exclusive with the Before attribute. A Before or After attribute is required when setting a Property.

**Before** (String)
  : The name of the standard or custom action before which this action should be performed. Mutually exclusive with the After attribute. A Before or After attribute is required when setting a Property.

**Id** (String)
  : This attribute specifies the Property to set to the Value.

**Sequence** (enumeration)
  : Controls which sequences the Property assignment is sequenced in. For 'execute', the assignment is scheduled in the InstallExecuteSequence. For 'ui', the assignment is scheduled in the InstallUISequence. For 'first', the assignment is scheduled in the InstallUISequence or the InstallExecuteSequence if the InstallUISequence is skipped at install time. For 'both', the assignment is scheduled in both the InstallUISequence and the InstallExecuteSequence. The default is 'both'. This attribute's value must be one of the following:
- *both*: Schedules the assignment in the InstallUISequence and the InstallExecuteSequence.
- *first*: Schedules the assignment to run in the InstallUISequence or the InstallExecuteSequence if the InstallUISequence is skipped.
- *execute*: Schedules the assignment only in the the InstallExecuteSequence.
- *ui*: Schedules the assignment only in the the InstallUISequence.

**Value** (String)
  : This attribute specifies a string value to assign to the Property. The value can be a literal value or derived from a Property element using the Formatted syntax.


## See also
[Custom](custom.md), [CustomActionRef](customactionref.md), [InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)