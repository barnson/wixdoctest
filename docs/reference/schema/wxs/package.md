---
custom_edit_url: null
sidebar_position: 157
---
# Package element
The Package element is analogous to the main function in a C program. When linking, only one Package section can be given to the linker to produce a successful result. Using this element creates an MSI file.

## Parents
[Wix](wix.md)

## Children
* [AdminExecuteSequence](adminexecutesequence.md) 
* [AdminUISequence](adminuisequence.md) 
* [AdvertiseExecuteSequence](advertiseexecutesequence.md) 
* [AppId](appid.md) 
* [Binary](binary.md) 
* [BroadcastEnvironmentChange (Util extension)](../util/broadcastenvironmentchange.md) 
* [BroadcastSettingChange (Util extension)](../util/broadcastsettingchange.md) 
* [CheckRebootRequired (Util extension)](../util/checkrebootrequired.md) 
* [CloseApplication (Util extension)](../util/closeapplication.md) 
* [ComplianceCheck](compliancecheck.md) 
* [ComPlusApplication (Complus extension)](../complus/complusapplication.md) 
* [ComPlusApplicationRole (Complus extension)](../complus/complusapplicationrole.md) 
* [ComPlusPartition (Complus extension)](../complus/compluspartition.md) 
* [ComPlusPartitionRole (Complus extension)](../complus/compluspartitionrole.md) 
* [Component](component.md) 
* [ComponentGroup](componentgroup.md) 
* [CustomAction](customaction.md) 
* [CustomActionRef](customactionref.md) 
* [CustomTable](customtable.md) 
* [CustomTableRef](customtableref.md) 
* [Directory](directory.md) 
* [DirectoryRef](directoryref.md) 
* [DotNetCompatibilityCheck (Netfx extension)](../netfx/dotnetcompatibilitycheck.md) 
* [DotNetCompatibilityCheckRef (Netfx extension)](../netfx/dotnetcompatibilitycheckref.md) 
* [EmbeddedChainer](embeddedchainer.md) 
* [EmbeddedChainerRef](embeddedchainerref.md) 
* [EnsureTable](ensuretable.md) 
* [ExitEarlyWithSuccess (Util extension)](../util/exitearlywithsuccess.md) 
* [FailWhenDeferred (Util extension)](../util/failwhendeferred.md) 
* [Feature](feature.md) 
* [FeatureGroupRef](featuregroupref.md) 
* [FeatureRef](featureref.md) 
* [FindVisualStudio (Vs extension)](../vs/findvisualstudio.md) 
* [GetCapabilities (Directx extension)](../directx/getcapabilities.md) 
* [Group (Util extension)](../util/group.md) 
* [Icon](icon.md) 
* [InstallExecuteSequence](installexecutesequence.md) 
* [InstallUISequence](installuisequence.md) 
* [InstanceTransforms](instancetransforms.md) 
* [Launch](launch.md) 
* [MajorUpgrade](majorupgrade.md) 
* [Media](media.md) 
* [MediaTemplate](mediatemplate.md) 
* [PackageCertificates](packagecertificates.md) 
* [PatchCertificates](patchcertificates.md) 
* [Property](property.md) 
* [PropertyRef](propertyref.md) 
* [QueryWindowsDirectories (Util extension)](../util/querywindowsdirectories.md) 
* [QueryWindowsDriverInfo (Util extension)](../util/querywindowsdriverinfo.md) 
* [QueryWindowsSuiteInfo (Util extension)](../util/querywindowssuiteinfo.md) 
* [QueryWindowsWellKnownSIDs (Util extension)](../util/querywindowswellknownsids.md) 
* [Requires](requires.md) 
* [RestartResource (Util extension)](../util/restartresource.md) 
* [SetDirectory](setdirectory.md) 
* [SetProperty](setproperty.md) 
* [SFPCatalog](sfpcatalog.md) 
* [SoftwareTag](softwaretag.md) 
* [SqlDatabase (Sql extension)](../sql/sqldatabase.md) 
* [StandardDirectory](standarddirectory.md) 
* [SummaryInformation](summaryinformation.md) 
* [SymbolPath](symbolpath.md) 
* [UI](ui.md) 
* [UIRef](uiref.md) 
* [Upgrade](upgrade.md) 
* [User (Util extension)](../util/user.md) 
* [WaitForEvent (Util extension)](../util/waitforevent.md) 
* [WaitForEventDeferred (Util extension)](../util/waitforeventdeferred.md) 
* [WebApplication (Iis extension)](../iis/webapplication.md) 
* [WebAppPool (Iis extension)](../iis/webapppool.md) 
* [WebDirProperties (Iis extension)](../iis/webdirproperties.md) 
* [WebLog (Iis extension)](../iis/weblog.md) 
* [WebSite (Iis extension)](../iis/website.md) 
* [WixUI (Ui extension)](../ui/wixui.md) 
* [WixVariable](wixvariable.md) 

## Remarks
<p>You can specify any valid Windows code page by integer like 1252, or by web name like Windows-1252. See [Code Pages](reference/codepage.md) for more information.</p>


## Attributes
**Codepage** (String)
  : The code page integer value or web name for the resulting MSI. See remarks for more information. The default codepage is 65001 (UTF-8).

**Compressed** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Indicates whether the package files are compressed. Default is compressed packages.

**InstallerVersion** (Integer)
  : The minimum version of the Windows Installer required to install this package. Take the major version of the required Windows Installer and multiply by a 100 then add the minor version of the Windows Installer. For example, "200" would represent Windows Installer 2.0 and "405" would represent Windows Installer 4.5. This value is defaulted to "500" which is the latest version of the Windows Installer and present in Windows 7 and later.

**Language** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'))
  : The decimal language ID (LCID) for the product.

**Manufacturer** (String, required)
  : The manufacturer of the package.

**Name** (String, required)
  : The descriptive name of the product.

**ProductCode** ([AutogenGuid](autogenguid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". A GUID can be auto-generated by setting the value to "*". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Optional ProductCode GUID for the package. By default, a new ProductCode will be generated with every build enabling major upgrades.

**Scope** (enumeration)
  : Use this attribute to specify the installation scope of this package: per-machine or per-user. This attribute's value must be one of the following:
- *perMachine*: Set this value to declare that the package is a per-machine installation and requires elevated privileges to install. Sets the ALLUSERS property to 1.
- *perUser*: Set this value to declare that the package is a per-user installation and does not require elevated privileges to install. Sets the package's InstallPrivileges attribute to "limited."

**ShortNames** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Indicates whether the package files are installed using 8.3 filenames.

**UpgradeCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : The upgrade code GUID for the product.

**Version** (String, required)
  : The product's version string.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)