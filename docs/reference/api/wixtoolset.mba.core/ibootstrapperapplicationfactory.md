---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBootstrapperApplicationFactory Interface
Interface used by WixToolset.Mba.Host to dynamically load the BA.
## Methods
| Method | Description |
| ------ | ----------- |
| [Create(pArgs, pResults)](#create_pargs_presults) | Low level method called by the native host. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Create(pArgs, pResults) Method {#create_pargs_presults}
Low level method called by the native host.
### Declaration
```cs
public void Create(
  System.IntPtr pArgs,
  System.IntPtr pResults
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| pArgs | System.IntPtr |  |
| pResults | System.IntPtr |  |
