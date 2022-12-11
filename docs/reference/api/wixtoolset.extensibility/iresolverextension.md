---
custom_edit_url: null
toc_max_heading_level: 2
---
# IResolverExtension Interface
Interface all resolver extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostResolve()](#postresolve_nop) | Called after all resolving occurs. |
| [PreResolve()](#preresolve_nop) | Called before resolving occurs. |
| [ResolveFile()](#resolvefile_nop) | Called to attempt to resolve source to a file. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostResolve() Method {#postresolve_nop}
Called after all resolving occurs.
### Declaration
```cs
public void PostResolve
```
## PreResolve() Method {#preresolve_nop}
Called before resolving occurs.
### Declaration
```cs
public void PreResolve
```
## ResolveFile() Method {#resolvefile_nop}
Called to attempt to resolve source to a file.
### Declaration
```cs
public Data.IResolveFileResult ResolveFile
```
