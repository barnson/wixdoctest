---
custom_edit_url: null
toc_max_heading_level: 2
---
# SummaryInfoRowCollection Class
Indexed container class for summary information rows.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetKeyForItem(row)](#getkeyforitem_row) | Gets the summary property ID for the _row_ . |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetKeyForItem(row) Method {#getkeyforitem_row}
Gets the summary property ID for the _row_ .
### Declaration
```cs
protected int GetKeyForItem(
  WixToolset.Data.WindowsInstaller.Row row
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| row | WixToolset.Data.WindowsInstaller.Row | The row to index. |
### Return value
`int` The summary property ID for the _row_ .
