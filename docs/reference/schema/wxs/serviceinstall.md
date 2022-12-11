---
custom_edit_url: null
sidebar_position: 241
---
# ServiceInstall element
Adds services for parent Component. Use the ServiceControl element to remove services.

## Windows Installer references
[ServiceInstall Table](https://docs.microsoft.com/en-us/windows/win32/msi/serviceinstall-table)

## Parents
[Component](component.md)

## Children
* [PermissionEx (Util extension)](../util/permissionex.md) 
* [ServiceConfig (Util extension)](../util/serviceconfig.md) 
* [ServiceConfigFailureActions](serviceconfigfailureactions.md) 
* [ServiceDependency](servicedependency.md) : Ordered list of dependencies when installing services.
* [UrlReservation (Http extension)](../http/urlreservation.md) 

## Remarks
The service executable installed will point to the KeyPath for the Component.
Therefore, you must ensure that the correct executable is either the first child
File element under this Component or explicitly mark the appropriate File element
as KeyPath='yes'.


## Attributes
**Account** (String)
  : Fully qualified names must be used even for local accounts, e.g.: ".\LOCAL_ACCOUNT". Valid only when ServiceType is ownProcess.

**Arguments** (String)
  : Contains any command line arguments or properties required to run the service.

**Description** (String)
  : Sets the description of the service.

**DisplayName** (String)
  : This column is the localizable string that user interface programs use to identify the service.

**EraseDescription** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Determines whether the existing service description will be ignored. If 'yes', the service description will be null, even if the Description attribute is set.

**ErrorControl** (enumeration, required)
  : Determines what action should be taken on an error. This attribute's value must be one of the following:
- *ignore*: Logs the error and continues with the startup operation.
- *normal*: Logs the error, displays a message box and continues the startup operation.
- *critical*: Logs the error if it is possible and the system is restarted with the last configuration known to be good. If the last-known-good configuration is being started, the startup operation fails.

**Id** (String)
  : Unique identifier for this service configuration. This value will default to the Name attribute if not specified.

**Interactive** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether or not the service interacts with the desktop.

**LoadOrderGroup** (String)
  : The load ordering group that this service should be a part of.

**Name** (String, required)
  : This column is the string that gives the service name to install.

**Password** (String)
  : The password for the account. Valid only when the account has a password.

**Start** (enumeration, required)
  : Determines when the service should be started. The Windows Installer does not support boot or system. This attribute's value must be one of the following:
- *auto*: The service will start during startup of the system.
- *demand*: The service will start when the service control manager calls the StartService function.
- *disabled*: The service can no longer be started.
- *boot*: The service is a device driver that will be started by the operating system boot loader. This value is not currently supported by the Windows Installer.
- *system*: The service is a device driver that will be started by the IoInitSystem function. This value is not currently supported by the Windows Installer.

**Type** (enumeration, required)
  : The Windows Installer does not currently support kernelDriver or systemDriver. This attribute's value must be one of the following:
- *ownProcess*: A Win32 service that runs its own process.
- *shareProcess*: A Win32 service that shares a process.
- *kernelDriver*: A kernel driver service. This value is not currently supported by the Windows Installer.
- *systemDriver*: A file system driver service. This value is not currently supported by the Windows Installer.

**Vital** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to 'yes' or left unspecified the overall install will fail if this service fails to install. A value of 'no' indicates failure to install the service will be ignored.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)