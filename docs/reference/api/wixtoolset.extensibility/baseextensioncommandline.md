---
custom_edit_url: null
toc_max_heading_level: 2
---
# BaseExtensionCommandLine Class
Base class for extensions to be able to parse the command-line.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetCommandLineHelp()](#getcommandlinehelp_nop) | See «see M:WixToolset.Extensibility.IExtensionCommandLine.GetCommandLineHelp»  |
| [PostParse()](#postparse_nop) | See «see M:WixToolset.Extensibility.IExtensionCommandLine.PostParse»  |
| [PreParse()](#preparse_nop) | See «see M:WixToolset.Extensibility.IExtensionCommandLine.PreParse(WixToolset.Extensibility.Data.ICommandLineContext)»  |
| [TryParseArgument()](#tryparseargument_nop) | See «see M:WixToolset.Extensibility.IExtensionCommandLine.TryParseArgument(WixToolset.Extensibility.Services.ICommandLineParser,System.String)»  |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetCommandLineHelp() Method {#getcommandlinehelp_nop}
See «see M:WixToolset.Extensibility.IExtensionCommandLine.GetCommandLineHelp» 
### Declaration
```cs
public Data.CommandLineHelp GetCommandLineHelp
```
## PostParse() Method {#postparse_nop}
See «see M:WixToolset.Extensibility.IExtensionCommandLine.PostParse» 
### Declaration
```cs
public void PostParse
```
## PreParse() Method {#preparse_nop}
See «see M:WixToolset.Extensibility.IExtensionCommandLine.PreParse(WixToolset.Extensibility.Data.ICommandLineContext)» 
### Declaration
```cs
public void PreParse
```
## TryParseArgument() Method {#tryparseargument_nop}
See «see M:WixToolset.Extensibility.IExtensionCommandLine.TryParseArgument(WixToolset.Extensibility.Services.ICommandLineParser,System.String)» 
### Declaration
```cs
public bool TryParseArgument
```
