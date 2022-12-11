---
custom_edit_url: null
sidebar_position: 237
---
# ServiceConfig element
Configures a service being installed or one that already exists. This element's functionality is available starting with MSI 5.0.

## Windows Installer references
[MsiServiceConfig Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiserviceconfig-table)

## Children
* [RequiredPrivilege](requiredprivilege.md) : List of privileges to apply to service.

## Attributes
**DelayedAutoStart** (String)
  : This attribute specifies whether an auto-start service should delay its start until after all other auto-start services. This attribute only affects auto-start services. Allowed values are "yes", "no" or a Formatted property that resolves to "1" (for "yes") or "0" (for "no"). If this attribute is not present the setting is not configured.

**FailureActionsWhen** (String)
  : This attribute specifies when failure actions should be applied. Allowed values are "failedToStop", "failedToStopOrReturnedError" or a Formatted property that resolves to "1" (for "failedToStopOrReturnedError") or "0" (for "failedToStop"). If this attribute is not present the setting is not configured.

**Id** (String)
  : Unique identifier for this service configuration. This value will default to the ServiceName attribute if not specified.

**OnInstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is installed. This attribute may be combined with OnReinstall and OnUninstall.

**OnReinstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is reinstalled. This attribute may be combined with OnInstall and OnUninstall.

**OnUninstall** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether to configure the service when the parent Component is uninstalled. This attribute may be combined with OnInstall and OnReinstall.

**PreShutdownDelay** (String)
  : This attribute specifies time in milliseconds that the Service Control Manager (SCM) waits after notifying the service of a system shutdown. If this attribute is not present the default value, 3 minutes, is used.

**ServiceName** (String)
  : Specifies the name of the service to configure. This value will default to the ServiceInstall/@Name attribute when nested under a ServiceInstall element.

**ServiceSid** (String)
  : Specifies the service SID to apply to the service. Valid values are "none", "restricted", "unrestricted" or a Formatted property that resolves to "0" (for "none"), "3" (for "restricted") or "1" (for "unrestricted"). If this attribute is not present the setting is not configured.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)