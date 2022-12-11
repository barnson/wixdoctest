---
custom_edit_url: null
sidebar_position: 216
---
# RemoveFolder element
Remove an empty folder if the parent component is selected for installation or removal. By default, the folder is the directory of the parent component. This can be overridden by specifying the Directory attribute with a value corresponding to the Id of the directory, or by specifying the Property attribute with a value corresponding to a property that will have a value that resolves to the full path of the folder.

## Windows Installer references
[RemoveFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/removefile-table)

## Parents
[Component](component.md)

## Attributes
**Directory** (String)
  : Overrides the directory of the parent component with a specific Directory. This Directory must exist in the installer database at creation time. This attribute cannot be specified in conjunction with the Property attribute.

**Id** (String)
  : Primary key used to identify this particular entry.

**On** (enumeration, required)
  : This value determines the time at which the folder may be removed, based on the install/uninstall of the parent component. For 'install', the folder will be removed only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource); for 'uninstall', the folder will be removed only when the parent component is being removed (msiInstallStateAbsent); for 'both', the folder will be removed in both cases. This attribute's value must be one of the following:
- *install*: The action should happen during install (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: The action should happen during uninstall (msiInstallStateAbsent).
- *both*: The action should happen during both install and uninstall.

**Property** (String)
  : Overrides the directory of the parent component with the value of the specified property. The property should have a value that resolves to the full path of the source directory. The property does not have to exist in the installer database at creation time; it could be created at installation time by a custom action, on the command line, etc. This attribute cannot be specified in conjunction with the Directory attribute.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute or parent Directory reference for the folder to be removed.


## See also
[CreateFolder](createfolder.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)