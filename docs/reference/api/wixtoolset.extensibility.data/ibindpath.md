---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBindPath Interface
Interface for a bind path.
## Properties
| Property | Description |
| ------ | ----------- |
| [Name](#name) | Name of the bind path or String.Empty if the path is unnamed. |
| [Path](#path) | Path for the bind path. |
| [Stage](#stage) | Stage for the bind path. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Name Property {#name}
Name of the bind path or String.Empty if the path is unnamed.
### Declaration
```cs
public string Name { get; set; } 
```
## Path Property {#path}
Path for the bind path.
### Declaration
```cs
public string Path { get; set; } 
```
## Stage Property {#stage}
Stage for the bind path.
### Declaration
```cs
public BindStage Stage { get; set; } 
```
