---
custom_edit_url: null
toc_max_heading_level: 2
---
# ICompilerExtension Interface
Interface all compiler extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostCompile()](#postcompile_nop) | Called at the end of the compilation of a source file. |
| [PreCompile()](#precompile_nop) | Called at the beginning of the compilation of a source file. |
## Properties
| Property | Description |
| ------ | ----------- |
| [Namespace](#namespace) | Gets the schema namespace for this extension. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostCompile() Method {#postcompile_nop}
Called at the end of the compilation of a source file.
### Declaration
```cs
public void PostCompile
```
## PreCompile() Method {#precompile_nop}
Called at the beginning of the compilation of a source file.
### Declaration
```cs
public void PreCompile
```
## Namespace Property {#namespace}
Gets the schema namespace for this extension.
### Declaration
```cs
public System.Xml.Linq.XNamespace Namespace { get; set; } 
```
