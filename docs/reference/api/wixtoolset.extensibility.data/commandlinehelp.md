---
custom_edit_url: null
toc_max_heading_level: 2
---
# CommandLineHelp Class
A command line option (switch or command) description.
## Properties
| Property | Description |
| ------ | ----------- |
| [Commands](#commands) | Optional list of command line commands. |
| [Description](#description) | Description for the command line option. |
| [Notes](#notes) | Optional additional notes for the command line option. |
| [Switches](#switches) | Optional list of command line switches. |
| [Usage](#usage) | Usage for the command line option. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Commands Property {#commands}
Optional list of command line commands.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.CommandLineHelpCommand> Commands { get; set; } 
```
## Description Property {#description}
Description for the command line option.
### Declaration
```cs
public string Description { get; set; } 
```
## Notes Property {#notes}
Optional additional notes for the command line option.
### Declaration
```cs
public string Notes { get; set; } 
```
## Switches Property {#switches}
Optional list of command line switches.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.CommandLineHelpSwitch> Switches { get; set; } 
```
## Usage Property {#usage}
Usage for the command line option.
### Declaration
```cs
public string Usage { get; set; } 
```
