---
custom_edit_url: null
sidebar_position: 39
---
# Component element
Component for parent Directory

## Windows Installer references
[Component Table](https://docs.microsoft.com/en-us/windows/win32/msi/component-table), [Condition Table](https://docs.microsoft.com/en-us/windows/win32/msi/condition-table), [Directory Table](https://docs.microsoft.com/en-us/windows/win32/msi/directory-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [ComponentGroup](componentgroup.md), [Directory](directory.md), [DirectoryRef](directoryref.md), [StandardDirectory](standarddirectory.md), [Feature](feature.md), [FeatureGroup](featuregroup.md), [FeatureRef](featureref.md)

## Children
* [AppId](appid.md) 
* [Category](category.md) 
* [Certificate (Iis extension)](../iis/certificate.md) 
* [Class](class.md) 
* [ComPlusApplication (Complus extension)](../complus/complusapplication.md) 
* [ComPlusApplicationRole (Complus extension)](../complus/complusapplicationrole.md) 
* [ComPlusAssembly (Complus extension)](../complus/complusassembly.md) 
* [ComPlusGroupInApplicationRole (Complus extension)](../complus/complusgroupinapplicationrole.md) 
* [ComPlusGroupInPartitionRole (Complus extension)](../complus/complusgroupinpartitionrole.md) 
* [ComPlusPartition (Complus extension)](../complus/compluspartition.md) 
* [ComPlusPartitionRole (Complus extension)](../complus/compluspartitionrole.md) 
* [ComPlusPartitionUser (Complus extension)](../complus/compluspartitionuser.md) 
* [ComPlusRoleForComponent (Complus extension)](../complus/complusroleforcomponent.md) 
* [ComPlusRoleForInterface (Complus extension)](../complus/complusroleforinterface.md) 
* [ComPlusRoleForMethod (Complus extension)](../complus/complusroleformethod.md) 
* [ComPlusSubscription (Complus extension)](../complus/complussubscription.md) 
* [ComPlusUserInApplicationRole (Complus extension)](../complus/complususerinapplicationrole.md) 
* [ComPlusUserInPartitionRole (Complus extension)](../complus/complususerinpartitionrole.md) 
* [CopyFile](copyfile.md) 
* [CreateFolder](createfolder.md) 
* [Driver (Difxapp extension)](../difxapp/driver.md) 
* [Environment](environment.md) 
* [EventSource (Util extension)](../util/eventsource.md) 
* [Extension](extension.md) 
* [File](file.md) 
* [FileShare (Util extension)](../util/fileshare.md) 
* [FirewallException (Firewall extension)](../firewall/firewallexception.md) 
* [IniFile](inifile.md) 
* [Interface](interface.md) 
* [InternetShortcut (Util extension)](../util/internetshortcut.md) 
* [IsolateComponent](isolatecomponent.md) 
* [MessageQueue (Msmq extension)](../msmq/messagequeue.md) 
* [MessageQueuePermission (Msmq extension)](../msmq/messagequeuepermission.md) 
* [ODBCDataSource](odbcdatasource.md) 
* [ODBCDriver](odbcdriver.md) 
* [ODBCTranslator](odbctranslator.md) 
* [PerformanceCategory (Util extension)](../util/performancecategory.md) 
* [ProgId](progid.md) 
* [Provides](provides.md) 
* [Registry](registry.md) 
* [RegistryKey](registrykey.md) 
* [RegistryValue](registryvalue.md) 
* [RemoveFile](removefile.md) 
* [RemoveFolder](removefolder.md) 
* [RemoveFolderEx (Util extension)](../util/removefolderex.md) 
* [RemoveRegistryKey](removeregistrykey.md) 
* [RemoveRegistryValue](removeregistryvalue.md) 
* [ReserveCost](reservecost.md) 
* [RestartResource (Util extension)](../util/restartresource.md) 
* [ServiceConfig (Util extension)](../util/serviceconfig.md) 
* [ServiceConfigFailureActions](serviceconfigfailureactions.md) 
* [ServiceControl](servicecontrol.md) 
* [ServiceInstall](serviceinstall.md) 
* [Shortcut](shortcut.md) 
* [SniSslCertificate (Http extension)](../http/snisslcertificate.md) 
* [SqlDatabase (Sql extension)](../sql/sqldatabase.md) 
* [SqlScript (Sql extension)](../sql/sqlscript.md) 
* [SqlString (Sql extension)](../sql/sqlstring.md) 
* [SymbolPath](symbolpath.md) 
* [TouchFile (Util extension)](../util/touchfile.md) 
* [TypeLib](typelib.md) 
* [UrlReservation (Http extension)](../http/urlreservation.md) 
* [User (Util extension)](../util/user.md) 
* [VsixPackage (Vs extension)](../vs/vsixpackage.md) 
* [WebAppPool (Iis extension)](../iis/webapppool.md) 
* [WebDir (Iis extension)](../iis/webdir.md) 
* [WebFilter (Iis extension)](../iis/webfilter.md) 
* [WebProperty (Iis extension)](../iis/webproperty.md) 
* [WebServiceExtension (Iis extension)](../iis/webserviceextension.md) 
* [WebSite (Iis extension)](../iis/website.md) 
* [WebVirtualDir (Iis extension)](../iis/webvirtualdir.md) 
* [XmlConfig (Util extension)](../util/xmlconfig.md) 
* [XmlFile (Util extension)](../util/xmlfile.md) 

## Attributes
**Bitness** ([BitnessTypeUnion](bitnesstype.md 'Values of this type will be "default", "always32" or "always64".'))
  : Overrides the default Component bitness. Only 64-bit Components an install to 64-bit locations such as `ProgramFiles64Folder` and the 64-bit registry. The value `always64` will force the Component bitness to be 64-bit and cannot be included in 32-bit packages. Simliarly, the value `always32` will force the Component bitness to 32-bit and can be included in 32-bit or 64-bit packages. The default value is `default` where the Component will be installed using the same bitness as the package.

**ComPlusFlags** (Integer)
  : Set this attribute to create a ComPlus entry. The value should be the export flags used during the generation of the .msi file. For more information see the COM+ documentation in the Platform SDK.

**Condition** (String)
  : The condition expression to be evaluated at install time. When false the Component will not be installed.

**Directory** (String)
  : Sets the Directory of the Component. If this element is nested under a Directory element, this value defaults to the value of the parent Directory/@Id.

**DisableRegistryReflection** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to 'yes' in order to disable registry reflection on all existing and new registry keys affected by this component. When set to 'yes', the Windows Installer calls the RegDisableReflectionKey on each key being accessed by the component. This bit is available with Windows Installer version 4.0 and is ignored on 32-bit systems.

**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : This attribute provides a default DiskId attribute for all child File elements. Specifying the DiskId on a Component element will override any DiskId attributes set by parent Directory or DirectoryRef elements. See the File element's DiskId attribute for more information about the purpose of the DiskId.

**Feature** (String)
  : Identifies a feature to which this component belongs, as a shorthand for a child ComponentRef element of the Feature element. The value of this attribute should correspond to the Id attribute of a Feature element authored elsewhere. Note that a single component can belong to multiple features but this attribute allows you to specify only a single feature.

**Guid** ([ComponentGuid](componentguid.md 'Values of this type must be a GUID, with or without braces: `01234567-89AB-CDEF-0123-456789ABCDEF` or `{01234567-89AB-CDEF-0123-456789ABCDEF}`. `PUT-GUID-HERE` can be used for sample code. Empty values are also supported.'))
  : This value should be a guid that uniquely identifies this component's contents, language, platform, and version. If omitted, the default value is '*' which indicates that the linker should generate a stable guid. Generatable guids are supported only for components with a single file as the component's keypath or no files and a registry value as the keypath. It's also possible to set the value to an empty string to specify an unmanaged component. Unmanaged components are a security vulnerability because the component cannot be removed or repaired by Windows Installer (it is essentially an unpatchable, permanent component). Therefore, a guid should always be specified for any component which contains resources that may need to be patched in the future.

**Id** (String)
  : Component identifier; this is the primary key for identifying components. If omitted, the compiler defaults the identifier to the identifier of the resource that is the explicit keypath of the component (for example, a child File element with KeyPath attribute with value 'yes'.

**KeyPath** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute's value is set to 'yes', then the Directory of this Component is used as the KeyPath. To set a Registry value or File as the KeyPath of a component, set the KeyPath attribute to 'yes' on one of those child elements. If KeyPath is not set to 'yes' for the Component or for a child Registry value or File, WiX will look at the child elements under the Component in sequential order and try to automatically select one of them as a key path. Allowing WiX to automatically select a key path can be dangerous because adding or removing child elements under the Component can inadvertantly cause the key path to change, which can lead to installation problems.

**Location** (enumeration)
  : Optional value that specifies the location that the component can be run from. This attribute's value must be one of the following:
- *local*: Prevents the component from running from the source or the network (this is the default behavior if this attribute is not set).
- *source*: Enforces that the component can only be run from the source (it cannot be run from the user's computer).
- *either*: Allows the component to run from source or locally.

**MultiInstance** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes', a new Component/@Guid will be generated for each instance transform. Ensure that all of the resources contained in a multi-instance Component will be installed to different paths based on the instance Property; otherwise, the Component Rules will be violated.

**NeverOverwrite** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes', the installer does not install or reinstall the component if a key path file or a key path registry entry for the component already exists. The application does register itself as a client of the component. Use this flag only for components that are being registered by the Registry table. Do not use this flag for components registered by the AppId, Class, Extension, ProgId, MIME, and Verb tables.

**Permanent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes', the installer does not remove the component during an uninstall. The installer registers an extra system client for the component in the Windows Installer registry settings (which basically just means that at least one product is always referencing this component). Note that this option differs from the behavior of not setting a guid because although the component is permanent, it is still patchable (because Windows Installer still tracks it), it's just not uninstallable.

**Shared** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute's value is set to 'yes', enables advanced patching semantics for Components that are shared across multiple MSI packages. Specifically, the Windows Installer will cache the shared files to improve patch uninstall. This functionality is available in Windows Installer 4.5 and later.

**SharedDllRefCount** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute's value is set to 'yes', the installer increments the reference count in the shared DLL registry of the component's key file. If this bit is not set, the installer increments the reference count only if the reference count already exists.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute or parent Directory reference where the Component will be installed.

**Transitive** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes', the installer reevaluates the value of the statement in the Condition upon a reinstall. If the value was previously False and has changed to True, the installer installs the component. If the value was previously True and has changed to False, the installer removes the component even if the component has other products as clients.

**UninstallWhenSuperseded** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes', the installer will uninstall the Component's files and registry keys when it is superseded by a patch. This functionality is available in Windows Installer 4.5 and later.


## See also
[ComponentRef](componentref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)