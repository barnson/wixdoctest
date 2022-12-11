---
custom_edit_url: null
sidebar_position: 86
---
# ExitCode element
Describes map of exit code returned from executable package to a bootstrapper behavior.

## Parents
[ExePackage](exepackage.md), [BundlePackage](bundlepackage.md)

## Attributes
**Behavior** (enumeration, required)
  : Choose one of the supported behaviors error codes: success, error, scheduleReboot, forceReboot, errorScheduleReboot, errorForceReboot. This attribute's value must be one of the following:
- *success*: The process completed successfully.
- *error*: The process failed.
- *scheduleReboot*: The process completed successfully and requires the machine to be restarted.
- *forceReboot*: The process completed successfully and initiated a restart.
- *errorScheduleReboot*: The process failed and requires the machine to be restarted.
- *errorForceReboot*: The process failed and initiated a restart.

**Value** (Integer)
  : Exit code returned from executable package. If no value is provided it means all values not explicitly set default to this behavior.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)