---
custom_edit_url: null
toc_max_heading_level: 2
---
# TrackedFileType Enumeration
Tracked file types.
## Members
| Member | Description |
| ------ | ----------- |
| BuiltContentOutput | Output created by the build process itself (like a .cab). These files can be recreated in the final output location by building again. |
| BuiltPdbOutput | Output pdb created by the build process itself (like a .wixpdb). These files can be recreated in the final output location by building again. |
| BuiltTargetOutput | Target output created by the build process itself (like a .msi, .msm, .wixlib, .exe). These files can be recreated in the final output location by building again. |
| CopiedOutput | Output copied by the build process (like external files in an .msi). These files are not created by the build process but are copied to the final output location. |
| Input | File tracked as input (like content included in an .msi). |
| Intermediate | Intermediate file (like a .cab in the cabcache). These are left for subsequent builds. |
| Temporary | Temporary file (like an .idt or any other temporary file). These are to be deleted before the build completes. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
