---
custom_edit_url: null
sidebar_position: 286
---
# ValidateProductID element
Sets the ProductID property to the full product identifier. This action must be sequenced before the user interface wizard in the InstallUISequence table and before the RegisterUser action in the InstallExecuteSequence table. If the product identifier has already been validated successfully, the ValidateProductID action does nothing. The ValidateProductID action always returns a success, whether or not the product identifier is valid, so that the product identifier can be entered on the command line the first time the product is run. The product identifier can be validated without having the user reenter this information by setting the PIDKEY property on the command line or by using a transform. The display of the dialog box requesting the user to enter the product identifier can then be made conditional upon the presence of the ProductID property, which is set when the PIDKEY property is validated. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[ValidateProductID Action](https://docs.microsoft.com/en-us/windows/win32/msi/validateproductid-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)