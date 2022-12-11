---
custom_edit_url: null
sidebar_position: 177
---
# Permission element
Sets ACLs on File, Registry, or CreateFolder. When under a Registry element, this cannot be used if the Action attribute's value is remove or removeKeyOnInstall. This element has no Id attribute. The table and key are taken from the parent element.

## Windows Installer references
[LockPermissions Table](https://docs.microsoft.com/en-us/windows/win32/msi/lockpermissions-table)

## Parents
[File](file.md), [RegistryKey](registrykey.md), [RegistryValue](registryvalue.md), [Registry](registry.md), [CreateFolder](createfolder.md)

## Attributes
**Append** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**ChangePermission** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**CreateChild** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : For a directory, the right to create a subdirectory. Only valid under a 'CreateFolder' parent.

**CreateFile** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : For a directory, the right to create a file in the directory. Only valid under a 'CreateFolder' parent.

**CreateLink** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**CreateSubkeys** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Delete** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**DeleteChild** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : For a directory, the right to delete a directory and all the files it contains, including read-only files. Only valid under a 'CreateFolder' parent.

**Domain** (String)
  : 

**EnumerateSubkeys** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Execute** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**FileAllRights** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Bit mask for FILE_ALL_ACCESS from WinNT.h (0x001F01FF).

**GenericAll** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**GenericExecute** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**GenericRead** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : specifying this will fail to grant read access

**GenericWrite** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Notify** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Read** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**ReadAttributes** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**ReadExtendedAttributes** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**ReadPermission** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**SpecificRightsAll** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Bit mask for SPECIFIC_RIGHTS_ALL from WinNT.h (0x0000FFFF).

**Synchronize** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**TakeOwnership** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Traverse** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : For a directory, the right to traverse the directory. By default, users are assigned the BYPASS_TRAVERSE_CHECKING privilege, which ignores the FILE_TRAVERSE access right. Only valid under a 'CreateFolder' parent.

**User** (String, required)
  : 

**Write** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**WriteAttributes** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**WriteExtendedAttributes** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)