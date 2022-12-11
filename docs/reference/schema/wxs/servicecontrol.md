---
custom_edit_url: null
sidebar_position: 239
---
# ServiceControl element
Starts, stops, and removes services for parent Component. This element is used to control the state of a service installed by the MSI or MSM file by using the start, stop and remove attributes. For example, Start='install' Stop='both' Remove='uninstall' would mean: start the service on install, remove the service when the product is uninstalled, and stop the service both on install and uninstall.

## Windows Installer references
[ServiceControl Table](https://docs.microsoft.com/en-us/windows/win32/msi/servicecontrol-table)

## Parents
[Component](component.md)

## Children
* [ServiceArgument](serviceargument.md) : Ordered list of arguments used when modifying services.

## Attributes
**Id** (String, required)
  : 

**Name** (String, required)
  : Name of the service.

**Remove** (enumeration)
  : Specifies whether the service should be removed by the DeleteServices action on install, uninstall or both. For 'install', the service will be removed only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource); for 'uninstall', the service will be removed only when the parent component is being removed (msiInstallStateAbsent); for 'both', the service will be removed in both cases. This attribute's value must be one of the following:
- *install*: The action should happen during install (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: The action should happen during uninstall (msiInstallStateAbsent).
- *both*: The action should happen during both install and uninstall.

**Start** (enumeration)
  : Specifies whether the service should be started by the StartServices action on install, uninstall or both. For 'install', the service will be started only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource); for 'uninstall', the service will be started only when the parent component is being removed (msiInstallStateAbsent); for 'both', the service will be started in both cases. This attribute's value must be one of the following:
- *install*: The action should happen during install (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: The action should happen during uninstall (msiInstallStateAbsent).
- *both*: The action should happen during both install and uninstall.

**Stop** (enumeration)
  : Specifies whether the service should be stopped by the StopServices action on install, uninstall or both. For 'install', the service will be stopped only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource); for 'uninstall', the service will be stopped only when the parent component is being removed (msiInstallStateAbsent); for 'both', the service will be stopped in both cases. This attribute's value must be one of the following:
- *install*: The action should happen during install (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: The action should happen during uninstall (msiInstallStateAbsent).
- *both*: The action should happen during both install and uninstall.

**Wait** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether or not to wait for the service to complete before continuing. The default is 'yes'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)