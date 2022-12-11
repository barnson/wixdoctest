---
custom_edit_url: null
sidebar_position: 34
---
# RemoveFolderEx element (Util extension)
Remove a folder and all contained files and folders if the parent component is selected for installation or removal. The folder must be specified in the Property attribute as the name of a property that will have a value that resolves to the full path of the folder before the CostInitialize action. Note that Directory ids cannot be used. For more details, see the Remarks.

## Windows Installer references
[RemoveFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/removefile-table)

## Parents
[Component](../wxs/component.md)

## Remarks
<p>
  The custom action that implements RemoveFolderEx does so by writing temporary rows to the RemoveFile table
  for each subfolder of the root folder you specify. Because it might dramatically affect Windows Installer's
  [File Costing](https://learn.microsoft.com/en-us/windows/win32/msi/file-costing),
  the temporary rows must be written before the CostInitialize standard action. Unfortunately, MSI doesn't
  create properties for the Directory hierarchy in your package until later, in the CostFinalize action.
</p>
<p>
  An easy workaround for a typical use case of removing a folder during uninstall is to write the directory
  path to the registry and to load it during uninstall. See [The WiX toolset's "Remember Property" pattern](http://robmensching.com/blog/posts/2010/5/2/the-wix-toolsets-remember-property-pattern)
  for an example.
</p>
<p>
  If you use custom actions to set properties, ensure that they are scheduled before the WixRemoveFoldersEx custom action.
</p>


## Attributes
**Condition** (String)
  : Condition that determines if the folders should be removed. Must be blank or evaluate to true for the folder to be scheduled for removal.

**Id** (String)
  : Primary key used to identify this particular entry. If this is not specified, a stable identifier will be generated at compile time based on the other attributes.

**On** (enumeration)
  : This value determines when the folder may be removed. This attribute's value must be one of the following:
- *install*: Removes the folder only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: Removes the folder only when the parent component is being removed (msiInstallStateAbsent). This is the default if the On attribute is not specified.
- *both*: Removes the folder when the parent component is being installed or removed.

**Property** (String)
  : The id of a property that resolves to the full path of the source directory.  The property does not have to exist in the installer database at creation time; it could be created at installation time by a custom action, on the command line, etc. The property value can contain environment variables surrounded by percent signs such as from a REG_EXPAND_SZ registry value; environment variables will be expanded before being evaluated for a full path.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)