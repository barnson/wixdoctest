---
custom_edit_url: null
sidebar_position: 80
---
# Environment element
Environment variables added or removed for the parent component.

## Windows Installer references
[Environment Table](https://docs.microsoft.com/en-us/windows/win32/msi/environment-table)

## Parents
[Component](component.md)

## Attributes
**Action** (enumeration)
  : Specfies whether the environmental variable should be created, set or removed when the parent component is installed. This attribute's value must be one of the following:
- *create*: Creates the environment variable if it does not exist, then set it during installation. This has no effect on the value of the environment variable if it already exists.
- *set*: Creates the environment variable if it does not exist, and then set it during installation. If the environment variable exists, set it during the installation.
- *remove*: Removes the environment variable during an installation. The installer only removes an environment variable during an installation if the name and value of the variable match the entries in the Name and Value attributes. If you want to remove an environment variable, regardless of its value, do not set the Value attribute.

**Id** (String, required)
  : Unique identifier for environment entry.

**Name** (String, required)
  : Name of the environment variable.

**Part** (enumeration)
  :  This attribute's value must be one of the following:
- *all*: This value is the entire environmental variable. This is the default.
- *first*: This value is prefixed.
- *last*: This value is appended.

**Permanent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies that the environment variable should not be removed on uninstall.

**Separator** (String)
  : Optional attribute to change the separator used between values. By default a semicolon is used.

**System** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies that the environment variable should be added to the system environment space. The default is 'no' which indicates the environment variable is added to the user environment space.

**Value** (String)
  : The value to set into the environment variable. If this attribute is not set, the environment variable is removed during installation if it exists on the machine.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)