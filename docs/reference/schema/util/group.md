---
custom_edit_url: null
sidebar_position: 18
---
# Group element (Util extension)
Finds user groups on the local machine or specified Active Directory domain. The local machine will be searched for the group first then fallback to looking in Active Directory. This element is not capable of creating new groups but can be used to add new or existing users to an existing group.

## Parents
[Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Attributes
**Domain** (String)
  : An optional [Formatted](https://learn.microsoft.com/en-us/windows/win32/msi/formatted) string that specifies the domain for the group.

**Id** (String)
  : Unique identifier in your installation package for this group.

**Name** (String, required)
  : A [Formatted](https://learn.microsoft.com/en-us/windows/win32/msi/formatted) string that contains the name of the group to be found.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)