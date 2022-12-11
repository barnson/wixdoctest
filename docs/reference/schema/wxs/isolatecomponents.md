---
custom_edit_url: null
sidebar_position: 125
---
# IsolateComponents element
Installs a copy of a component (commonly a shared DLL) into a private location for use by a specific application (typically an .exe). This isolates the application from other copies of the component that may be installed to a shared location on the computer. The action refers to each record of the IsolatedComponent table and associates the files of the component listed in the Component_Shared field with the component listed in the Component_Application field. The installer installs the files of Component_Shared into the same directory as Component_Application. The installer generates a file in this directory, zero bytes in length, having the short filename name of the key file for Component_Application (typically this is the same file name as the .exe) appended with .local. The IsolatedComponent action does not affect the installation of Component_Application. Uninstalling Component_Application also removes the Component_Shared files and the .local file from the directory. The IsolateComponents action can be used only in the InstallUISequence table and the InstallExecuteSequence table. This action must come after the CostInitialize action and before the CostFinalize action. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[IsolateComponents Action](https://docs.microsoft.com/en-us/windows/win32/msi/isolatecomponents-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

## See also
[IsolateComponent](isolatecomponent.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)