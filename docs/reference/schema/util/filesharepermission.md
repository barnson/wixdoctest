---
custom_edit_url: null
sidebar_position: 16
---
# FileSharePermission element (Util extension)
Sets ACLs on a FileShare. This element has no Id attribute. The table and key are taken from the parent element.

## Parents
[FileShare](fileshare.md)

## Attributes
**ChangePermission** (wxs:YesNoTypeUnion)
  : 

**CreateChild** (wxs:YesNoTypeUnion)
  : For a directory, the right to create a subdirectory.  Only valid under a 'CreateFolder' parent.

**CreateFile** (wxs:YesNoTypeUnion)
  : For a directory, the right to create a file in the directory.  Only valid under a 'CreateFolder' parent.

**Delete** (wxs:YesNoTypeUnion)
  : 

**DeleteChild** (wxs:YesNoTypeUnion)
  : For a directory, the right to delete a directory and all the files it contains, including read-only files.  Only valid under a 'CreateFolder' parent.

**GenericAll** (wxs:YesNoTypeUnion)
  : 

**GenericExecute** (wxs:YesNoTypeUnion)
  : 

**GenericRead** (wxs:YesNoTypeUnion)
  : specifying this will fail to grant read access

**GenericWrite** (wxs:YesNoTypeUnion)
  : 

**Read** (wxs:YesNoTypeUnion)
  : 

**ReadAttributes** (wxs:YesNoTypeUnion)
  : 

**ReadExtendedAttributes** (wxs:YesNoTypeUnion)
  : 

**ReadPermission** (wxs:YesNoTypeUnion)
  : 

**Synchronize** (wxs:YesNoTypeUnion)
  : 

**TakeOwnership** (wxs:YesNoTypeUnion)
  : 

**Traverse** (wxs:YesNoTypeUnion)
  : For a directory, the right to traverse the directory.  By default, users are assigned the BYPASS_TRAVERSE_CHECKING privilege, which ignores the FILE_TRAVERSE access right.  Only valid under a 'CreateFolder' parent.

**User** (String, required)
  : 

**WriteAttributes** (wxs:YesNoTypeUnion)
  : 

**WriteExtendedAttributes** (wxs:YesNoTypeUnion)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)