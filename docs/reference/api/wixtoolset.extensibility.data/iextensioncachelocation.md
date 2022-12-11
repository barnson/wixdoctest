---
custom_edit_url: null
toc_max_heading_level: 2
---
# IExtensionCacheLocation Interface
Location where extensions may be cached.
## Properties
| Property | Description |
| ------ | ----------- |
| [Path](#path) | Path for the extension cache location. |
| [Scope](#scope) | Scope for the extension cache location. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Path Property {#path}
Path for the extension cache location.
### Declaration
```cs
public string Path { get; set; } 
```
## Scope Property {#scope}
Scope for the extension cache location.
### Declaration
```cs
public ExtensionCacheLocationScope Scope { get; set; } 
```
