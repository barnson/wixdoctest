---
custom_edit_url: null
sidebar_position: 9
---
# AppSearch element
Uses file signatures to search for existing versions of products. The AppSearch action may use this information to determine where upgrades are to be installed. The AppSearch action can also be used to set a property to the existing value of an registry or .ini file entry. AppSearch should be authored into the InstallUISequence table and InstallExecuteSequence table. The installer prevents The AppSearch action from running in the InstallExecuteSequence sequence if the action has already run in InstallUISequence sequence. The AppSearch action searches for file signatures using the CompLocator table first, the RegLocator table next, then the IniLocator table, and finally the DrLocator table. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[AppSearch Table](https://docs.microsoft.com/en-us/windows/win32/msi/appsearch-table), [AppSearch Action](https://docs.microsoft.com/en-us/windows/win32/msi/appsearch-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

## See also
[ComponentSearch](componentsearch.md), [FileSearch](filesearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)