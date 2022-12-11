---
custom_edit_url: null
sidebar_position: 213
---
# RemoveExistingProducts element
Goes through the product codes listed in the ActionProperty column of the Upgrade table and removes the products in sequence. Special actions don't have a built-in sequence number and thus must appear relative to another action. The suggested way to do this is by using the Before or After attribute. InstallExecute and InstallExecuteAgain can optionally appear anywhere between InstallInitialize and InstallFinalize.

## Windows Installer references
[RemoveExistingProducts Action](https://docs.microsoft.com/en-us/windows/win32/msi/removeexistingproducts-action)

## Parents
[InstallExecuteSequence](installexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)