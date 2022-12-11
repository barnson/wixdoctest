---
custom_edit_url: null
toc_max_heading_level: 2
---
# VerUtilVersionReleaseLabel Class
A release label from a «see T:WixToolset.Mba.Core.VerUtilVersion» .
## Properties
| Property | Description |
| ------ | ----------- |
| [IsNumeric](#isnumeric) | Whether the label was parsed as a number. |
| [Label](#label) | The string version of the label. |
| [Value](#value) | If «see P:WixToolset.Mba.Core.VerUtilVersionReleaseLabel.IsNumeric» then the value that was parsed. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## IsNumeric Property {#isnumeric}
Whether the label was parsed as a number.
### Declaration
```cs
public bool IsNumeric { get; set; } 
```
## Label Property {#label}
The string version of the label.
### Declaration
```cs
public string Label { get; set; } 
```
## Value Property {#value}
If «see P:WixToolset.Mba.Core.VerUtilVersionReleaseLabel.IsNumeric» then the value that was parsed.
### Declaration
```cs
public System.UInt32 Value { get; set; } 
```
