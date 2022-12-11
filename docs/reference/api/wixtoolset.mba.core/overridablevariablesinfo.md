---
custom_edit_url: null
toc_max_heading_level: 2
---
# OverridableVariablesInfo Class
Default implementation of «see T:WixToolset.Mba.Core.IOverridableVariables» .
## Methods
| Method | Description |
| ------ | ----------- |
| [ParseFromXml(root)](#parsefromxml_root) | Parses the overridable variable info from the BA manifest. |
## Properties
| Property | Description |
| ------ | ----------- |
| [CommandLineType](#commandlinetype) |  |
| [Variables](#variables) |  |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ParseFromXml(root) Method {#parsefromxml_root}
Parses the overridable variable info from the BA manifest.
### Declaration
```cs
public static IOverridableVariables ParseFromXml(
  System.Xml.XPath.XPathNavigator root
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| root | System.Xml.XPath.XPathNavigator | XML root |
### Return value
`IOverridableVariables` The parsed information.
## CommandLineType Property {#commandlinetype}

### Declaration
```cs
public VariableCommandLineType CommandLineType { get; set; } 
```
## Variables Property {#variables}

### Declaration
```cs
public System.Collections.Generic.IDictionary<System.String,WixToolset.Mba.Core.IOverridableVariableInfo> Variables { get; set; } 
```
