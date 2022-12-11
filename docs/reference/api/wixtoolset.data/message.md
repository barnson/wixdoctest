---
custom_edit_url: null
toc_max_heading_level: 2
---
# Message Class
Event args for message events.
## Methods
| Method | Description |
| ------ | ----------- |
| [ElevateToError()](#elevatetoerror_nop) | Changes the message into an error message. |
## Properties
| Property | Description |
| ------ | ----------- |
| [Id](#id) | Gets the Id for the message. |
| [Level](#level) | Gets or sets the «see T:WixToolset.Data.MessageLevel» for the message. |
| [MessageArgs](#messageargs) | Gets the arguments for the format string. |
| [ResourceManager](#resourcemanager) | Gets the resource manager for this event args. |
| [ResourceNameOrFormat](#resourcenameorformat) | Gets the name of the resource or format string if no resource manager was provided. |
| [SourceLineNumbers](#sourcelinenumbers) | Gets the source line numbers. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ElevateToError() Method {#elevatetoerror_nop}
Changes the message into an error message.
### Declaration
```cs
public void ElevateToError
```
## Id Property {#id}
Gets the Id for the message.
### Declaration
```cs
public int Id { get; set; } 
```
## Level Property {#level}
Gets or sets the «see T:WixToolset.Data.MessageLevel» for the message.
### Declaration
```cs
public MessageLevel Level { get; set; } 
```
## MessageArgs Property {#messageargs}
Gets the arguments for the format string.
### Declaration
```cs
public System.Object[] MessageArgs { get; set; } 
```
## ResourceManager Property {#resourcemanager}
Gets the resource manager for this event args.
### Declaration
```cs
public System.Resources.ResourceManager ResourceManager { get; set; } 
```
## ResourceNameOrFormat Property {#resourcenameorformat}
Gets the name of the resource or format string if no resource manager was provided.
### Declaration
```cs
public string ResourceNameOrFormat { get; set; } 
```
## SourceLineNumbers Property {#sourcelinenumbers}
Gets the source line numbers.
### Declaration
```cs
public SourceLineNumber SourceLineNumbers { get; set; } 
```
