---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILayoutExtension Interface
Interface all layout extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostLayout()](#postlayout_nop) | Called after all layout occurs. |
| [PreLayout()](#prelayout_nop) | Called before layout occurs. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostLayout() Method {#postlayout_nop}
Called after all layout occurs.
### Declaration
```cs
public void PostLayout
```
## PreLayout() Method {#prelayout_nop}
Called before layout occurs.
### Declaration
```cs
public void PreLayout
```
