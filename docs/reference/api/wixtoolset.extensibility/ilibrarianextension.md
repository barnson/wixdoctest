---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILibrarianExtension Interface
Interface all librarian extensions implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [PostCombine(result)](#postcombine_result) | Called at the end of combining. |
| [PreCombine(context)](#precombine_context) | Called at the beginning of combining. |
| [ResolveFile(sourceLineNumber, symbolDefinition, path)](#resolvefile_sourcelinenumber_symboldefinition_path) | Resolves a path to a file path on disk. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PostCombine(result) Method {#postcombine_result}
Called at the end of combining.
### Declaration
```cs
public void PostCombine(
  Data.ILibraryResult result
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| result | Data.ILibraryResult | Combined library result. |
## PreCombine(context) Method {#precombine_context}
Called at the beginning of combining.
### Declaration
```cs
public void PreCombine(
  Data.ILibraryContext context
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| context | Data.ILibraryContext | Librarian context. |
## ResolveFile(sourceLineNumber, symbolDefinition, path) Method {#resolvefile_sourcelinenumber_symboldefinition_path}
Resolves a path to a file path on disk.
### Declaration
```cs
public Data.IResolveFileResult ResolveFile(
  WixToolset.Data.SourceLineNumber sourceLineNumber,
  WixToolset.Data.IntermediateSymbolDefinition symbolDefinition,
  string path
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| sourceLineNumber | WixToolset.Data.SourceLineNumber | Source line number for the path to resolve. |
| symbolDefinition | WixToolset.Data.IntermediateSymbolDefinition | Symbol related to the path to resolve. |
| path | string | Path to resolve. |
### Return value
`Data.IResolveFileResult` Optional resolved file result.
