---
custom_edit_url: null
sidebar_position: 20
---
# Bundle element
The root element for creating bundled packages.

## Parents
[Wix](wix.md)

## Children
* [ApprovedExeForElevation](approvedexeforelevation.md) 
* [BootstrapperApplication](bootstrapperapplication.md) 
* [BootstrapperApplicationRef](bootstrapperapplicationref.md) 
* [BundleCustomData](bundlecustomdata.md) 
* [BundleCustomDataRef](bundlecustomdataref.md) 
* [BundleExtension](bundleextension.md) 
* [BundleExtensionRef](bundleextensionref.md) 
* [Chain](chain.md) 
* [CloseApplication (Util extension)](../util/closeapplication.md) 
* [ComponentSearch (Util extension)](../util/componentsearch.md) 
* [ComponentSearchRef (Util extension)](../util/componentsearchref.md) 
* [Condition (Bal extension)](../bal/condition.md) 
* [Container](container.md) 
* [ContainerRef](containerref.md) 
* [DirectorySearch (Util extension)](../util/directorysearch.md) 
* [DirectorySearchRef (Util extension)](../util/directorysearchref.md) 
* [DotNetCoreSearch (Netfx extension)](../netfx/dotnetcoresearch.md) 
* [DotNetCoreSearchRef (Netfx extension)](../netfx/dotnetcoresearchref.md) 
* [FileSearch (Util extension)](../util/filesearch.md) 
* [FileSearchRef (Util extension)](../util/filesearchref.md) 
* [Log](log.md) 
* [ManagedBootstrapperApplicationPrereqInformation (Bal extension)](../bal/managedbootstrapperapplicationprereqinformation.md) 
* [OptionalUpdateRegistration](optionalupdateregistration.md) 
* [PayloadGroup](payloadgroup.md) 
* [PayloadGroupRef](payloadgroupref.md) 
* [ProductSearch (Util extension)](../util/productsearch.md) 
* [ProductSearchRef (Util extension)](../util/productsearchref.md) 
* [RegistrySearch (Util extension)](../util/registrysearch.md) 
* [RegistrySearchRef (Util extension)](../util/registrysearchref.md) 
* [RelatedBundle](relatedbundle.md) 
* [Requires](requires.md) 
* [SetVariable](setvariable.md) 
* [SetVariableRef](setvariableref.md) 
* [SoftwareTag](softwaretag.md) 
* [Update](update.md) 
* [Variable](variable.md) 
* [WindowsFeatureSearch (Util extension)](../util/windowsfeaturesearch.md) 
* [WindowsFeatureSearchRef (Util extension)](../util/windowsfeaturesearchref.md) 
* [WixVariable](wixvariable.md) 

## Attributes
**AboutUrl** (String)
  : A URL for more information about the bundle to display in Programs and Features (also known as Add/Remove Programs).

**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Whether Packages and Payloads not assigned to a container should be added to the default attached container or if they should be external. The default is yes.

**Condition** (String)
  : The condition of the bundle. If the condition is not met, the bundle will refuse to run. Conditions are checked before the bootstrapper application is loaded (before detect), and thus can only reference built-in variables such as variables which indicate the version of the OS.

**Copyright** (String)
  : The legal copyright found in the version resources of final bundle executable. If this attribute is not provided the copyright will be set to "Copyright (c) [Bundle/@Manufacturer]. All rights reserved.".

**DisableModify** ([YesNoButtonTypeUnion](yesnobuttontype.md 'Values of this type will either be "button", "yes"/"true", or "no"/"false".'))
  : Determines whether the bundle can be modified via the Programs and Features (also known as Add/Remove Programs). If the value is "button" then Programs and Features will show a single "Uninstall/Change" button. If the value is "yes" then Programs and Features will only show the "Uninstall" button". If the value is "no", the default, then a "Change" button is shown. See the DisableRemove attribute for information how to not display the bundle in Programs and Features.

**DisableRemove** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Determines whether the bundle can be removed via the Programs and Features (also known as Add/Remove Programs). If the value is "yes" then the "Uninstall" button will not be displayed. The default is "no" which ensures there is an "Uninstall" button to remove the bundle. If the "DisableModify" attribute is also "yes" or "button" then the bundle will not be displayed in Progams and Features and another mechanism (such as registering as a related bundle addon) must be used to ensure the bundle can be removed.

**HelpTelephone** (String)
  : A telephone number for help to display in Programs and Features (also known as Add/Remove Programs).

**HelpUrl** (String)
  : A URL to the help for the bundle to display in Programs and Features (also known as Add/Remove Programs).

**IconSourceFile** (String)
  : Path to an icon that will replace the default icon in the final Bundle executable. This icon will also be displayed in Programs and Features (also known as Add/Remove Programs).

**InProgressName** (String)
  : Optional name to display in Add/Remove Programs while the bundle is being installed, uninstalled, repaired.

**Manufacturer** (String)
  : The publisher of the bundle to display in Programs and Features (also known as Add/Remove Programs).

**Name** (String)
  : The name of the bundle to display in Programs and Features (also known as Add/Remove Programs). This name can be accessed and overwritten by a BootstrapperApplication using the WixBundleName bundle variable.

**ParentName** (String)
  : The name of the parent bundle to display in Installed Updates (also known as Add/Remove Programs). This name is used to nest or group bundles that will appear as updates. If the parent name does not actually exist, a virtual parent is created automatically.

**ProviderKey** (String)
  : Optional attribute to explicitly author the provider key for the entire bundle.  This provider key is designed to persist throughout compatible upgrades so that dependent bundles do not have to be reinstalled and will not prevent your product from being upgraded. If this attribute is not authored, the value is the automatically-generated bundle ID and will not automatically support upgrades.   Only a single provider key is supported for bundles. To author that your bundle provides additional features via packages, author different provider keys for your packages.

**SplashScreenSourceFile** (String)
  : Path to a bitmap that will be shown as the bootstrapper application is being loaded. If this attribute is not specified, no splash screen will be displayed.

**Tag** (String)
  : Set this string to uniquely identify this bundle to its own BA, and to related bundles. The value of this string only matters to the BA, and its value has no direct effect on engine functionality.

**UpdateUrl** (String)
  : A URL for updates of the bundle to display in Programs and Features (also known as Add/Remove Programs).

**UpgradeCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : Unique identifier for a family of bundles. If two bundles have the same UpgradeCode the bundle with the highest version will be installed.

**Version** (String, required)
  : The version of the bundle. Newer versions upgrade earlier versions of the bundles with matching UpgradeCodes. If the bundle is registered in Programs and Features then this attribute will be displayed in the Programs and Features user interface.

**CommandLineVariables** (enumeration)
  : This value determines whether case sensitivity is used to match overridable variables specified on the command line. The default is "caseSensitive". This attribute's value must be one of the following:
- *caseSensitive*
- *caseInsensitive*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)