---
custom_edit_url: null
sidebar_position: 10
---
# EventSource element (Util extension)
Creates an event source.

## Parents
[Component](../wxs/component.md)

## Attributes
**CategoryCount** (Integer)
  : The number of categories in CategoryMessageFile. CategoryMessageFile must be specified too.

**CategoryMessageFile** (String)
  : Name of the category message file. CategoryCount must be specified too. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed. It is also written as a REG_EXPAND_SZ string, so you can use %environment_variable% syntax to refer to a file already present on the user's machine.

**EventMessageFile** (String, required)
  : Name of the event message file. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed. It is also written as a REG_EXPAND_SZ string, so you can use %environment_variable% syntax to refer to a file already present on the user's machine.

**KeyPath** (wxs:YesNoTypeUnion)
  : Marks the EventSource registry as the key path of the component it belongs to.

**Log** (String, required)
  : Name of the event source's log. The "Security" log is not support.

**Name** (String, required)
  : Name of the event source.

**ParameterMessageFile** (String)
  : Name of the parameter message file. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed. It is also written as a REG_EXPAND_SZ string, so you can use %environment_variable% syntax to refer to a file already present on the user's machine.

**SupportsErrors** (wxs:YesNoTypeUnion)
  : Equivalent to EVENTLOG_ERROR_TYPE.

**SupportsFailureAudits** (wxs:YesNoTypeUnion)
  : Equivalent to EVENTLOG_AUDIT_FAILURE.

**SupportsInformationals** (wxs:YesNoTypeUnion)
  : Equivalent to EVENTLOG_INFORMATION_TYPE.

**SupportsSuccessAudits** (wxs:YesNoTypeUnion)
  : Equivalent to EVENTLOG_AUDIT_SUCCESS.

**SupportsWarnings** (wxs:YesNoTypeUnion)
  : Equivalent to EVENTLOG_WARNING_TYPE.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)