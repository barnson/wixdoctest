---
custom_edit_url: null
toc_max_heading_level: 2
---
# Installation Class
Subclasses of this abstract class represent a unique instance of a registered product or patch installation.
## Properties
| Property | Description |
| ------ | ----------- |
| [Context](#context) | Gets the user context of this product or patch installation. |
| [IsInstalled](#isinstalled) | Gets a value indicating whether this product or patch is installed on the current system. |
| [Item](#item) | Gets a property about the product or patch installation. |
| [SourceList](#sourcelist) | Gets the source list of this product or patch installation. |
| [UserSid](#usersid) | Gets the user security identifier (SID) under which this product or patch installation is available. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Context Property {#context}
Gets the user context of this product or patch installation.
### Declaration
```cs
public UserContexts Context { get; set; } 
```
## IsInstalled Property {#isinstalled}
Gets a value indicating whether this product or patch is installed on the current system.
### Declaration
```cs
public bool IsInstalled { get; set; } 
```
## Item Property {#item}
Gets a property about the product or patch installation.
### Declaration
```cs
public string Item[
  string propertyName
] { get; set; } 
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| propertyName | string | Name of the property being retrieved. |
## SourceList Property {#sourcelist}
Gets the source list of this product or patch installation.
### Declaration
```cs
public SourceList SourceList { get; set; } 
```
## UserSid Property {#usersid}
Gets the user security identifier (SID) under which this product or patch installation is available.
### Declaration
```cs
public string UserSid { get; set; } 
```
