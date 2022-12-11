---
custom_edit_url: null
toc_max_heading_level: 2
---
# BootstrapperApplicationData Class
Utility class for reading BootstrapperApplicationData.xml.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetAttribute(node, attributeName)](#getattribute_node_attributename) | Utility method for parsing BootstrapperApplicationData.xml. |
| [GetYesNoAttribute(node, attributeName)](#getyesnoattribute_node_attributename) | Utility method for parsing BootstrapperApplicationData.xml. |
## Properties
| Property | Description |
| ------ | ----------- |
| [BADataFile](#badatafile) |  |
| [Bundle](#bundle) |  |
## Fields
| Field | Description |
| ------ | ----------- |
| DefaultFile | The default path to BootstrapperApplicationData.xml. |
| DefaultFileName |  |
| DefaultFolder | The default path of where the BA was extracted to. |
| XMLNamespace |  |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetAttribute(node, attributeName) Method {#getattribute_node_attributename}
Utility method for parsing BootstrapperApplicationData.xml.
### Declaration
```cs
public static string GetAttribute(
  System.Xml.XPath.XPathNavigator node,
  string attributeName
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| node | System.Xml.XPath.XPathNavigator |  |
| attributeName | string |  |
## GetYesNoAttribute(node, attributeName) Method {#getyesnoattribute_node_attributename}
Utility method for parsing BootstrapperApplicationData.xml.
### Declaration
```cs
public static System.Nullable<System.Boolean> GetYesNoAttribute(
  System.Xml.XPath.XPathNavigator node,
  string attributeName
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| node | System.Xml.XPath.XPathNavigator |  |
| attributeName | string |  |
## BADataFile Property {#badatafile}

### Declaration
```cs
public System.IO.FileInfo BADataFile { get; set; } 
```
## Bundle Property {#bundle}

### Declaration
```cs
public IBundleInfo Bundle { get; set; } 
```
