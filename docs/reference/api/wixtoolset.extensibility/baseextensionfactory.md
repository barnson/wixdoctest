---
custom_edit_url: null
toc_max_heading_level: 2
---
# BaseExtensionFactory Class
Base class for extension factories. Implementations may request an IWixToolsetCoreServiceProvider at instantiation by having a single parameter constructor for it.
## Properties
| Property | Description |
| ------ | ----------- |
| [ExtensionTypes](#extensiontypes) | The extension types of the WiX extension. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ExtensionTypes Property {#extensiontypes}
The extension types of the WiX extension.
### Declaration
```cs
protected System.Collections.Generic.IReadOnlyCollection<System.Type> ExtensionTypes { get; set; } 
```
