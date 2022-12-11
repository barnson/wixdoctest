---
custom_edit_url: null
toc_max_heading_level: 2
---
# CustomActionAttribute Class
Marks a method as a custom action entry point.
## Properties
| Property | Description |
| ------ | ----------- |
| [Name](#name) | Gets or sets the name of the custom action entrypoint. A null value defaults to the name of the method. |
### Remarks
A custom action method must be defined as public and static, take a single «see T:WixToolset.Dtf.WindowsInstaller.Session» object as a parameter, and return an «see T:WixToolset.Dtf.WindowsInstaller.ActionResult» enumeration value.

`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Name Property {#name}
Gets or sets the name of the custom action entrypoint. A null value defaults to the name of the method.
### Declaration
```cs
public string Name { get; set; } 
```
