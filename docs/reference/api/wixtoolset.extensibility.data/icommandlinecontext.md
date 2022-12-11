---
custom_edit_url: null
toc_max_heading_level: 2
---
# ICommandLineContext Interface
Command-line context.
## Properties
| Property | Description |
| ------ | ----------- |
| [Arguments](#arguments) | Command-line arguments. |
| [ExtensionManager](#extensionmanager) | Extension manager. |
| [ServiceProvider](#serviceprovider) | Service provider. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Arguments Property {#arguments}
Command-line arguments.
### Declaration
```cs
public ICommandLineArguments Arguments { get; set; } 
```
## ExtensionManager Property {#extensionmanager}
Extension manager.
### Declaration
```cs
public WixToolset.Extensibility.Services.IExtensionManager ExtensionManager { get; set; } 
```
## ServiceProvider Property {#serviceprovider}
Service provider.
### Declaration
```cs
public System.IServiceProvider ServiceProvider { get; set; } 
```
