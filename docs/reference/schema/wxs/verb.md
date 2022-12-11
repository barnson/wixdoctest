---
custom_edit_url: null
sidebar_position: 288
---
# Verb element
Verb definition for an Extension. When advertised, this element creates a row in the Verb table. When not advertised, this element creates the appropriate rows in Registry table.

## Windows Installer references
[Verb Table](https://docs.microsoft.com/en-us/windows/win32/msi/verb-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table)

## Parents
[Extension](extension.md)

## Attributes
**Argument** (String)
  : Value for the command arguments. Note that the resolution of properties in the Argument field is limited. A property formatted as [Property] in this field can only be resolved if the property already has the intended value when the component owning the verb is installed. For example, for the argument "[#MyDoc.doc]" to resolve to the correct value, the same process must be installing the file MyDoc.doc and the component that owns the verb.

**Command** (String)
  : The localized text displayed on the context menu.

**Id** (String, required)
  : The verb for the command.

**Sequence** (Integer)
  : The sequence of the commands. Only verbs for which the Sequence is specified are used to prepare an ordered list for the default value of the shell key. The Verb with the lowest value in this column becomes the default verb. Used only for Advertised verbs.

**TargetFile** (String)
  : Either this attribute or the TargetProperty attribute must be specified for a non-advertised verb. The value should be the identifier of the target file to be executed for the verb.

**TargetProperty** (String)
  : Either this attribute or the TargetFile attribute must be specified for a non-advertised verb. The value should be the identifier of the property which will resolve to the path to the target file to be executed for the verb.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)