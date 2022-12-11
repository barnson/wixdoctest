---
custom_edit_url: null
sidebar_position: 36
---
# ServiceConfig element (Util extension)
Service configuration information for failure actions.

## Parents
[Component](../wxs/component.md), [ServiceInstall](../wxs/serviceinstall.md)

## Remarks
<dl>
  <dd>Nesting a ServiceConfig element under a ServiceInstall element will result in the service being installed to be configured.</dd>
  <dd>Nesting a ServiceConfig element under a component element will result in an already installed service to be configured. If the service does not exist prior to the install of the MSI package, the install will fail.</dd>
</dl>


## Attributes
**FirstFailureActionType** (enumeration, required)
  : Action to take on the first failure of the service. This attribute's value must be one of the following:
- *none*
- *reboot*
- *restart*
- *runCommand*

**ProgramCommandLine** (String)
  : If any of the three *ActionType attributes is "runCommand", this specifies the command to run when doing so.  This value is formatted.

**RebootMessage** (String)
  : If any of the three *ActionType attributes is "reboot", this specifies the message to broadcast to server users before doing so.

**ResetPeriodInDays** (Integer)
  : Number of days after which to reset the failure count to zero if there are no failures.

**RestartServiceDelayInSeconds** (Integer)
  : If any of the three *ActionType attributes is "restart", this specifies the number of seconds to wait before doing so.

**SecondFailureActionType** (enumeration, required)
  : Action to take on the second failure of the service. This attribute's value must be one of the following:
- *none*
- *reboot*
- *restart*
- *runCommand*

**ServiceName** (String)
  : Required if not under a ServiceInstall element.

**ThirdFailureActionType** (enumeration, required)
  : Action to take on the third failure of the service. This attribute's value must be one of the following:
- *none*
- *reboot*
- *restart*
- *runCommand*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)