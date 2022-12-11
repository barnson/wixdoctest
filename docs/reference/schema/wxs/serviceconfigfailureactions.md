---
custom_edit_url: null
sidebar_position: 238
---
# ServiceConfigFailureActions element
Configures the failure actions for a service being installed or one that already exists. This element's functionality is available starting with MSI 5.0.

## Windows Installer references
[MsiServiceConfigFailureActions Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiserviceconfigfailureactions-table)

## Parents
[ServiceInstall](serviceinstall.md), [Component](component.md)

## Children
* [Failure](failure.md) : Ordered list of failure actions to apply to service.

## Attributes
**Command** (String)
  : This attribute specifies command to execute when a "runCommand" failure action hit. If an empty string is provided it clears the existing command. If this attribute is not present the setting is not changed.

**Id** (String)
  : Unique identifier for this service configuration. This value will default to the ServiceName attribute if not specified.

**OnInstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is installed. This attribute may be combined with OnReinstall and OnUninstall.

**OnReinstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is reinstalled. This attribute may be combined with OnInstall and OnUninstall.

**OnUninstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is uninstalled. This attribute may be combined with OnInstall and OnReinstall.

**RebootMessage** (String)
  : Specifies the message to show for a reboot failure action. If an empty string is provided it clears any existing reboot message. If this attribute is not present the setting is not changed.

**ResetPeriod** (String)
  : Specifies the time in seconds to reset the failure count. If this attribute is not present the failure count will not be reset.

**ServiceName** (String)
  : Specifies the name of the service to configure. This value will default to the ServiceInstall/@Name attribute when nested under a ServiceInstall element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)