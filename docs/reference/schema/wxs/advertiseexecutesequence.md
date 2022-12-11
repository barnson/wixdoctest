---
custom_edit_url: null
sidebar_position: 3
---
# AdvertiseExecuteSequence element


## Windows Installer references
[AdvtExecuteSequence Table](https://docs.microsoft.com/en-us/windows/win32/msi/advtexecutesequence-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Children
* [CostFinalize](costfinalize.md) : Ends the internal installation costing process begun by the CostInitialize action.
* [CostInitialize](costinitialize.md) : Initiates the internal installation costing process.
* [CreateShortcuts](createshortcuts.md) : Manages the creation of shortcuts.
* [Custom](custom.md) : Use to sequence a custom action. The only custom actions that are allowed in the AdvtExecuteSequence are type 19 (0x013) type 35 (0x023) and type 51 (0x033).
* [InstallFinalize](installfinalize.md) : Marks the end of a sequence of actions that change the system.
* [InstallInitialize](installinitialize.md) : Marks the beginning of a sequence of actions that change the system.
* [InstallValidate](installvalidate.md) : Verifies that all costed volumes have enough space for the installation.
* [MsiPublishAssemblies](msipublishassemblies.md) : Manages the advertisement of CLR and Win32 assemblies.
* [PublishComponents](publishcomponents.md) : Manages the advertisement of the components from the PublishComponent table.
* [PublishFeatures](publishfeatures.md) : Writes each feature's state into the system registry.
* [PublishProduct](publishproduct.md) : Manages the advertisement of the product information with the system.
* [RegisterClassInfo](registerclassinfo.md) : Manages the registration of COM class information with the system.
* [RegisterExtensionInfo](registerextensioninfo.md) : Manages the registration of extension related information with the system.
* [RegisterMIMEInfo](registermimeinfo.md) : Registers MIME-related registry information with the system.
* [RegisterProgIdInfo](registerprogidinfo.md) : Manages the registration of OLE ProgId information with the system.

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)