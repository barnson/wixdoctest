---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBinderExtension Interface
Interface all binder extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostBind()](#postbind_nop) | Called after all binding occurs. |
| [PreBind()](#prebind_nop) | Called before binding occurs. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostBind() Method {#postbind_nop}
Called after all binding occurs.
### Declaration
```cs
public void PostBind
```
## PreBind() Method {#prebind_nop}
Called before binding occurs.
### Declaration
```cs
public void PreBind
```
