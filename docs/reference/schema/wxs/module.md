---
custom_edit_url: null
sidebar_position: 140
---
# Module element
The Module element is analogous to the main function in a C program. When linking, only one Module section can be given to the linker to produce a successful result. Using this element creates an msm file.

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
* [ComPlusApplication (Complus extension)](../complus/complusapplication.md) 
* [ComPlusApplicationRole (Complus extension)](../complus/complusapplicationrole.md) 
* [ComPlusPartition (Complus extension)](../complus/compluspartition.md) 
* [ComPlusPartitionRole (Complus extension)](../complus/compluspartitionrole.md) 
* [Component](component.md) 
* [ComponentGroupRef](componentgroupref.md) 
* [ComponentRef](componentref.md) 
* [Configuration](configuration.md) 
* [CustomAction](customaction.md) 
* [CustomActionRef](customactionref.md) 
* [CustomTable](customtable.md) 
* [CustomTableRef](customtableref.md) 
* [Dependency](dependency.md) 
* [Directory](directory.md) 
* [DirectoryRef](directoryref.md) 
* [DotNetCompatibilityCheck (Netfx extension)](../netfx/dotnetcompatibilitycheck.md) 
* [DotNetCompatibilityCheckRef (Netfx extension)](../netfx/dotnetcompatibilitycheckref.md) 
* [EmbeddedChainer](embeddedchainer.md) 
* [EmbeddedChainerRef](embeddedchainerref.md) 
* [EnsureTable](ensuretable.md) 
* [Exclusion](exclusion.md) 
* [ExitEarlyWithSuccess (Util extension)](../util/exitearlywithsuccess.md) 
* [FailWhenDeferred (Util extension)](../util/failwhendeferred.md) 
* [FindVisualStudio (Vs extension)](../vs/findvisualstudio.md) 
* [GetCapabilities (Directx extension)](../directx/getcapabilities.md) 
* [Group (Util extension)](../util/group.md) 
* [Icon](icon.md) 
* [IgnoreTable](ignoretable.md) 
* [InstallExecuteSequence](installexecutesequence.md) 
* [InstallUISequence](installuisequence.md) 
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
* [SqlDatabase (Sql extension)](../sql/sqldatabase.md) 
* [StandardDirectory](standarddirectory.md) 
* [Substitution](substitution.md) 
* [SummaryInformation](summaryinformation.md) 
* [UI](ui.md) 
* [UIRef](uiref.md) 
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

## Attributes
**Codepage** (String)
  : The code page integer value or web name for the resulting MSM. You can specify any valid Windows code by by integer like 1252, or by web name like Windows-1252. See [Code pages](reference/codepage.md) for more information.

**Guid** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : The GUID of the Merge Module that will be appended to primary keys in the database.

**Id** (String, required)
  : The name of the merge module (not the file name).

**InstallerVersion** (Integer)
  : The minimum version of the Windows Installer required to install this package. Take the major version of the required Windows Installer and multiply by a 100 then add the minor version of the Windows Installer. For example, "200" would represent Windows Installer 2.0 and "405" would represent Windows Installer 4.5. This value is defaulted to "500" which is the latest version of the Windows Installer and present in Windows 7 and later.

**Language** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : The decimal language ID (LCID) of the merge module.

**Version** (String, required)
  : The major and minor versions of the merge module.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)