---
custom_edit_url: null
toc_max_heading_level: 2
---
# IVariableResolution Interface
Result when resolving a variable.
## Properties
| Property | Description |
| ------ | ----------- |
| [DelayedResolve](#delayedresolve) | Indicates if the value contains variables that cannot be resolved yet. |
| [IsDefault](#isdefault) | Indicates whether a bind variables default value was used in the resolution. |
| [UpdatedValue](#updatedvalue) | Indicates whether the resolution updated the value. |
| [Value](#value) | The resolved value. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## DelayedResolve Property {#delayedresolve}
Indicates if the value contains variables that cannot be resolved yet.
### Declaration
```cs
public bool DelayedResolve { get; set; } 
```
## IsDefault Property {#isdefault}
Indicates whether a bind variables default value was used in the resolution.
### Declaration
```cs
public bool IsDefault { get; set; } 
```
## UpdatedValue Property {#updatedvalue}
Indicates whether the resolution updated the value.
### Declaration
```cs
public bool UpdatedValue { get; set; } 
```
## Value Property {#value}
The resolved value.
### Declaration
```cs
public string Value { get; set; } 
```
