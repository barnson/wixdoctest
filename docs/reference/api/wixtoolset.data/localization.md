---
custom_edit_url: null
toc_max_heading_level: 2
---
# Localization Class
Object that represents a localization file.
## Properties
| Property | Description |
| ------ | ----------- |
| [Codepage](#codepage) | Gets the codepage. |
| [Culture](#culture) | Gets the culture. |
| [LocalizedControls](#localizedcontrols) | Gets the localized controls. |
| [SummaryInformationCodepage](#summaryinformationcodepage) | Gets the summary information codepage. |
| [Variables](#variables) | Gets the variables. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Codepage Property {#codepage}
Gets the codepage.
### Declaration
```cs
public System.Nullable<System.Int32> Codepage { get; set; } 
```
## Culture Property {#culture}
Gets the culture.
### Declaration
```cs
public string Culture { get; set; } 
```
## LocalizedControls Property {#localizedcontrols}
Gets the localized controls.
### Declaration
```cs
public System.Collections.Generic.ICollection<System.Collections.Generic.KeyValuePair`2<System.String,WixToolset.Data.LocalizedControl>> LocalizedControls { get; set; } 
```
## SummaryInformationCodepage Property {#summaryinformationcodepage}
Gets the summary information codepage.
### Declaration
```cs
public System.Nullable<System.Int32> SummaryInformationCodepage { get; set; } 
```
## Variables Property {#variables}
Gets the variables.
### Declaration
```cs
public System.Collections.Generic.ICollection<WixToolset.Data.Bind.BindVariable> Variables { get; set; } 
```
