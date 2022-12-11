---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILinkerExtension Interface
Interface all linker extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostLink()](#postlink_nop) | Called after all linking occurs. |
| [PreLink()](#prelink_nop) | Called before linking occurs. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostLink() Method {#postlink_nop}
Called after all linking occurs.
### Declaration
```cs
public void PostLink
```
## PreLink() Method {#prelink_nop}
Called before linking occurs.
### Declaration
```cs
public void PreLink
```
