---
custom_edit_url: null
toc_max_heading_level: 2
---
# ICommandLineArguments Interface
Parsed command-line arguments.
## Methods
| Method | Description |
| ------ | ----------- |
| [Parse()](#parse_nop) | Parses this arguments after it is populated. |
| [Populate(commandLine)](#populate_commandline) | Populate this argument from a string. |
| [Populate(args)](#populate_args) | Populate this argument from array of strings. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Parse() Method {#parse_nop}
Parses this arguments after it is populated.
### Declaration
```cs
public WixToolset.Extensibility.Services.ICommandLineParser Parse
```
### Return value
`WixToolset.Extensibility.Services.ICommandLineParser` Parser for this arguments.
## Populate(commandLine) Method {#populate_commandline}
Populate this argument from a string.
### Declaration
```cs
public void Populate(
  string commandLine
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| commandLine | string | String to parse. |
## Populate(args) Method {#populate_args}
Populate this argument from array of strings.
### Declaration
```cs
public void Populate(
  System.String[] args
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| args | System.String[] | Array of strings. |
