---
custom_edit_url: null
sidebar_position: 113
---
# InstallExecuteSequence element


## Windows Installer references
[InstallExecuteSequence Table](https://docs.microsoft.com/en-us/windows/win32/msi/installexecutesequence-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Children
* [AllocateRegistrySpace](allocateregistryspace.md) : Ensures the needed amount of space exists in the registry.
* [AppSearch](appsearch.md) : Uses file signatures to search for existing versions of products.
* [BindImage](bindimage.md) : Binds each executable or DLL that must be bound to the DLLs imported by it.
* [CCPSearch](ccpsearch.md) : Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed.
* [CostFinalize](costfinalize.md) : Ends the internal installation costing process begun by the CostInitialize action.
* [CostInitialize](costinitialize.md) : Initiates the internal installation costing process.
* [CreateFolders](createfolders.md) : Creates empty folders for components that are set to be installed.
* [CreateShortcuts](createshortcuts.md) : Manages the creation of shortcuts.
* [Custom](custom.md) : Use to sequence a custom action.
* [DeleteServices](deleteservices.md) : Stops a service and removes its registration from the system.
* [DisableRollback](disablerollback.md) : Disables rollback for the remainder of the installation.
* [DuplicateFiles](duplicatefiles.md) : Duplicates files installed by the InstallFiles action.
* [FileCost](filecost.md) : Initiates dynamic costing of standard installation actions.
* [FindRelatedProducts](findrelatedproducts.md) : Runs through each record of the Upgrade table in sequence and compares the upgrade code, product version, and language in each row to products installed on the system.
* [ForceReboot](forcereboot.md) : Prompts the user for a restart of the system during the installation. Not fixed sequence.
* [InstallExecute](installexecute.md) : Runs a script containing all operations spooled since either the start of the installation or the last InstallExecute action, or InstallExecuteAgain action.
* [InstallExecuteAgain](installexecuteagain.md) : Runs a script containing all operations spooled since either the start of the installation or the last InstallExecute action, or InstallExecuteAgain action.
* [InstallFiles](installfiles.md) : Copies files specified in the File table from the source directory to the destination directory.
* [InstallFinalize](installfinalize.md) : Marks the end of a sequence of actions that change the system.
* [InstallInitialize](installinitialize.md) : Marks the beginning of a sequence of actions that change the system.
* [InstallODBC](installodbc.md) : Installs the drivers, translators, and data sources in the ODBCDriver table, ODBCTranslator table, and ODBCDataSource table.
* [InstallServices](installservices.md) : Registers a service for the system.
* [InstallValidate](installvalidate.md) : Verifies that all costed volumes have enough space for the installation.
* [IsolateComponents](isolatecomponents.md) : Installs a copy of a component (commonly a shared DLL) into a private location for use by a specific application (typically an .exe).
* [LaunchConditions](launchconditions.md) : Queries the LaunchCondition table and evaluates each conditional statement recorded there.
* [MigrateFeatureStates](migratefeaturestates.md) : Used for upgrading or installing over an existing application.
* [MoveFiles](movefiles.md) : Locates existing files on the system and moves or copies those files to a new location.
* [MsiPublishAssemblies](msipublishassemblies.md) : Manages the advertisement of CLR and Win32 assemblies.
* [MsiUnpublishAssemblies](msiunpublishassemblies.md) : Manages the unadvertisement of CLR and Win32 assemblies that are being removed.
* [PatchFiles](patchfiles.md) : Queries the Patch table to determine which patches are to be applied.
* [ProcessComponents](processcomponents.md) : Registers and unregisters components, their key paths, and the component clients.
* [PublishComponents](publishcomponents.md) : Manages the advertisement of the components from the PublishComponent table.
* [PublishFeatures](publishfeatures.md) : Writes each feature's state into the system registry.
* [PublishProduct](publishproduct.md) : Manages the advertisement of the product information with the system.
* [RegisterClassInfo](registerclassinfo.md) : Manages the registration of COM class information with the system.
* [RegisterComPlus](registercomplus.md) : Registers COM+ applications.
* [RegisterExtensionInfo](registerextensioninfo.md) : Manages the registration of extension related information with the system.
* [RegisterFonts](registerfonts.md) : Registers installed fonts with the system.
* [RegisterMIMEInfo](registermimeinfo.md) : Registers MIME-related registry information with the system.
* [RegisterProduct](registerproduct.md) : Registers the product information with the installer.
* [RegisterProgIdInfo](registerprogidinfo.md) : Manages the registration of OLE ProgId information with the system.
* [RegisterTypeLibraries](registertypelibraries.md) : Registers type libraries with the system.
* [RegisterUser](registeruser.md) : Registers the user information with the installer to identify the user of a product.
* [RemoveDuplicateFiles](removeduplicatefiles.md) : Deletes files installed by the DuplicateFiles action.
* [RemoveEnvironmentStrings](removeenvironmentstrings.md) : Modifies the values of environment variables.
* [RemoveExistingProducts](removeexistingproducts.md) : Goes through the product codes listed in the ActionProperty column of the Upgrade table and removes the products in sequence.
* [RemoveFiles](removefiles.md) : Removes files previously installed by the InstallFiles action.
* [RemoveFolders](removefolders.md) : Removes any folders linked to components set to be removed or run from source.
* [RemoveIniValues](removeinivalues.md) : Removes .ini file information specified for removal in the RemoveIniFile table if the component is set to be installed locally or run from source.
* [RemoveODBC](removeodbc.md) : Removes the data sources, translators, and drivers listed for removal during the installation.
* [RemoveRegistryValues](removeregistryvalues.md) : Removes a registry value that has been authored into the registry table if the associated component was installed locally or as run from source, and is now set to be uninstalled.
* [RemoveShortcuts](removeshortcuts.md) : Manages the removal of an advertised shortcut whose feature is selected for uninstallation or a nonadvertised shortcut whose component is selected for uninstallation.
* [ResolveSource](resolvesource.md) : Determines the location of the source and sets the SourceDir property if the source has not been resolved yet. Not fixed sequence.
* [RMCCPSearch](rmccpsearch.md) : Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed.
* [ScheduleReboot](schedulereboot.md) : Prompts the user to restart the system at the end of installation. Not fixed sequence.
* [SelfRegModules](selfregmodules.md) : Processes all modules listed in the SelfReg table and registers all installed modules with the system.
* [SelfUnregModules](selfunregmodules.md) : Unregisters all modules listed in the SelfReg table that are scheduled to be uninstalled.
* [SetODBCFolders](setodbcfolders.md) : Checks for existing ODBC drivers and sets the target directory for each new driver to the location of an existing driver.
* [StartServices](startservices.md) : Starts system services.
* [StopServices](stopservices.md) : Stops system services.
* [UnpublishComponents](unpublishcomponents.md) : Manages the unadvertisement of components listed in the PublishComponent table.
* [UnpublishFeatures](unpublishfeatures.md) : Removes selection-state and feature-component mapping information from the registry.
* [UnregisterClassInfo](unregisterclassinfo.md) : Manages the removal of COM class information from the system registry.
* [UnregisterComPlus](unregistercomplus.md) : Removes COM+ applications from the registry.
* [UnregisterExtensionInfo](unregisterextensioninfo.md) : Manages the removal of extension-related information from the system registry.
* [UnregisterFonts](unregisterfonts.md) : Removes registration information about installed fonts from the system.
* [UnregisterMIMEInfo](unregistermimeinfo.md) : Unregisters MIME-related registry information from the system.
* [UnregisterProgIdInfo](unregisterprogidinfo.md) : Manages the unregistration of OLE ProgId information with the system.
* [UnregisterTypeLibraries](unregistertypelibraries.md) : Unregisters type libraries from the system.
* [ValidateProductID](validateproductid.md) : Sets the ProductID property to the full product identifier.
* [WriteEnvironmentStrings](writeenvironmentstrings.md) : Modifies the values of environment variables.
* [WriteIniValues](writeinivalues.md) : Writes the .ini file information that the application needs written to its .ini files.
* [WriteRegistryValues](writeregistryvalues.md) : Sets up an application's registry information.

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)