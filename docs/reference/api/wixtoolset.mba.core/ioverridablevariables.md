---
custom_edit_url: null
toc_max_heading_level: 2
---
# IOverridableVariables Interface
Overridable variable information from the BA manifest.
## Properties
| Property | Description |
| ------ | ----------- |
| [CommandLineType](#commandlinetype) | The «see T:WixToolset.Mba.Core.VariableCommandLineType» of the bundle. |
| [Variables](#variables) | Variable Dictionary of variable name to «see T:WixToolset.Mba.Core.IOverridableVariableInfo» . |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CommandLineType Property {#commandlinetype}
The «see T:WixToolset.Mba.Core.VariableCommandLineType» of the bundle.
### Declaration
```cs
public VariableCommandLineType CommandLineType { get; set; } 
```
## Variables Property {#variables}
Variable Dictionary of variable name to «see T:WixToolset.Mba.Core.IOverridableVariableInfo» .
### Declaration
```cs
public System.Collections.Generic.IDictionary<System.String,WixToolset.Mba.Core.IOverridableVariableInfo> Variables { get; set; } 
```
