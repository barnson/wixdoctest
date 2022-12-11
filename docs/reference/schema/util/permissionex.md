---
custom_edit_url: null
sidebar_position: 25
---
# PermissionEx element (Util extension)
Sets ACLs on File, Registry, CreateFolder, or ServiceInstall.  When under a Registry element, this cannot be used if the Action attribute's value is remove or removeKeyOnInstall.  This element has no Id attribute. The table and key are taken from the parent element.

## Parents
[CreateFolder](../wxs/createfolder.md), [File](../wxs/file.md), [Registry](../wxs/registry.md), [RegistryKey](../wxs/registrykey.md), [RegistryValue](../wxs/registryvalue.md), [ServiceInstall](../wxs/serviceinstall.md)

## Attributes
**Append** (wxs:YesNoTypeUnion)
  : 

**ChangePermission** (wxs:YesNoTypeUnion)
  : 

**CreateChild** (wxs:YesNoTypeUnion)
  : For a directory, the right to create a subdirectory.  Only valid under a 'CreateFolder' parent.

**CreateFile** (wxs:YesNoTypeUnion)
  : For a directory, the right to create a file in the directory.  Only valid under a 'CreateFolder' parent.

**CreateLink** (wxs:YesNoTypeUnion)
  : 

**CreateSubkeys** (wxs:YesNoTypeUnion)
  : 

**Delete** (wxs:YesNoTypeUnion)
  : 

**DeleteChild** (wxs:YesNoTypeUnion)
  : For a directory, the right to delete a directory and all the files it contains, including read-only files.  Only valid under a 'CreateFolder' parent.

**Domain** (String)
  : 

**EnumerateSubkeys** (wxs:YesNoTypeUnion)
  : 

**Execute** (wxs:YesNoTypeUnion)
  : 

**GenericAll** (wxs:YesNoTypeUnion)
  : 

**GenericExecute** (wxs:YesNoTypeUnion)
  : 

**GenericRead** (wxs:YesNoTypeUnion)
  : specifying this will fail to grant read access

**GenericWrite** (wxs:YesNoTypeUnion)
  : 

**Inheritable** (wxs:YesNoTypeUnion)
  : Whether the permissions are inheritable. The default is "yes".

**Notify** (wxs:YesNoTypeUnion)
  : 

**Read** (wxs:YesNoTypeUnion)
  : 

**ReadAttributes** (wxs:YesNoTypeUnion)
  : 

**ReadExtendedAttributes** (wxs:YesNoTypeUnion)
  : 

**ReadPermission** (wxs:YesNoTypeUnion)
  : 

**ServiceChangeConfig** (wxs:YesNoTypeUnion)
  : Required to call the ChangeServiceConfig or ChangeServiceConfig2 function to change the service configuration.  Only valid under a 'ServiceInstall' parent.

**ServiceEnumerateDependents** (wxs:YesNoTypeUnion)
  : Required to call the EnumDependentServices function to enumerate all the services dependent on the service.  Only valid under a 'ServiceInstall' parent.

**ServiceInterrogate** (wxs:YesNoTypeUnion)
  : Required to call the ControlService function to ask the service to report its status immediately.  Only valid under a 'ServiceInstall' parent.

**ServicePauseContinue** (wxs:YesNoTypeUnion)
  : Required to call the ControlService function to pause or continue the service.  Only valid under a 'ServiceInstall' parent.

**ServiceQueryConfig** (wxs:YesNoTypeUnion)
  : Required to call the QueryServiceConfig and QueryServiceConfig2 functions to query the service configuration.  Only valid under a 'ServiceInstall' parent.

**ServiceQueryStatus** (wxs:YesNoTypeUnion)
  : Required to call the QueryServiceStatus function to ask the service control manager about the status of the service.  Only valid under a 'ServiceInstall' parent.

**ServiceStart** (wxs:YesNoTypeUnion)
  : Required to call the StartService function to start the service.  Only valid under a 'ServiceInstall' parent.

**ServiceStop** (wxs:YesNoTypeUnion)
  : Required to call the ControlService function to stop the service.  Only valid under a 'ServiceInstall' parent.

**ServiceUserDefinedControl** (wxs:YesNoTypeUnion)
  : Required to call the ControlService function to specify a user-defined control code.  Only valid under a 'ServiceInstall' parent.

**Synchronize** (wxs:YesNoTypeUnion)
  : 

**TakeOwnership** (wxs:YesNoTypeUnion)
  : 

**Traverse** (wxs:YesNoTypeUnion)
  : For a directory, the right to traverse the directory.  By default, users are assigned the BYPASS_TRAVERSE_CHECKING privilege, which ignores the FILE_TRAVERSE access right.  Only valid under a 'CreateFolder' parent.

**User** (String, required)
  : 

**Write** (wxs:YesNoTypeUnion)
  : 

**WriteAttributes** (wxs:YesNoTypeUnion)
  : 

**WriteExtendedAttributes** (wxs:YesNoTypeUnion)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)