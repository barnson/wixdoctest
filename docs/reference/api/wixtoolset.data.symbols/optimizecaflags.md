---
custom_edit_url: null
toc_max_heading_level: 2
---
# OptimizeCAFlags Enumeration
Values for the OptimizeCA MsiPatchMetdata property, which indicates whether custom actions can be skipped when applying the patch.
## Members
| Member | Description |
| ------ | ----------- |
| None | No custom actions are skipped. |
| SkipAssignment | Skip property (type 51) and directory (type 35) assignment custom actions. |
| SkipDeferred | Skip custom actions that run within the script. |
| SkipImmediate | Skip immediate custom actions that are not property or directory assignment custom actions. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
