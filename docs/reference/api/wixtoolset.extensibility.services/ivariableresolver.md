---
custom_edit_url: null
toc_max_heading_level: 2
---
# IVariableResolver Interface

## Methods
| Method | Description |
| ------ | ----------- |
| [AddVariable(sourceLineNumber, name, value, overridable)](#addvariable_sourcelinenumber_name_value_overridable) | Add a variable. |
| [ResolveVariables(sourceLineNumbers, value)](#resolvevariables_sourcelinenumbers_value) | Resolve the wix variables in a value. |
| [ResolveVariables(sourceLineNumbers, value, errorOnUnknown)](#resolvevariables_sourcelinenumbers_value_erroronunknown) | Resolve the wix variables in a value. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## AddVariable(sourceLineNumber, name, value, overridable) Method {#addvariable_sourcelinenumber_name_value_overridable}
Add a variable.
### Declaration
```cs
public void AddVariable(
  WixToolset.Data.SourceLineNumber sourceLineNumber,
  string name,
  string value,
  bool overridable
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| sourceLineNumber | WixToolset.Data.SourceLineNumber | The source line information for the value. |
| name | string | The name of the variable. |
| value | string | The value of the variable. |
| overridable | bool | Indicates whether the variable can be overridden by an existing variable. |
## ResolveVariables(sourceLineNumbers, value) Method {#resolvevariables_sourcelinenumbers_value}
Resolve the wix variables in a value.
### Declaration
```cs
public IVariableResolution ResolveVariables(
  WixToolset.Data.SourceLineNumber sourceLineNumbers,
  string value
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| sourceLineNumbers | WixToolset.Data.SourceLineNumber | The source line information for the value. |
| value | string | The value to resolve. |
### Return value
`IVariableResolution` The resolved result.
## ResolveVariables(sourceLineNumbers, value, errorOnUnknown) Method {#resolvevariables_sourcelinenumbers_value_erroronunknown}
Resolve the wix variables in a value.
### Declaration
```cs
public IVariableResolution ResolveVariables(
  WixToolset.Data.SourceLineNumber sourceLineNumbers,
  string value,
  bool errorOnUnknown
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| sourceLineNumbers | WixToolset.Data.SourceLineNumber | The source line information for the value. |
| value | string | The value to resolve. |
| errorOnUnknown | bool | true if unknown variables should throw errors. |
### Return value
`IVariableResolution` The resolved value.
