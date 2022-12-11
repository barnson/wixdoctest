---
custom_edit_url: null
sidebar_position: 95
---
# File element
File specification for File table, must be child node of Component.

## Windows Installer references
[File Table](https://docs.microsoft.com/en-us/windows/win32/msi/file-table)

## Parents
[Component](component.md)

## Children
* [AppId](appid.md) 
* [AssemblyName](assemblyname.md) 
* [Class](class.md) 
* [CopyFile](copyfile.md) : Used to create a duplicate of this file elsewhere.
* [EventManifest (Util extension)](../util/eventmanifest.md) 
* [FirewallException (Firewall extension)](../firewall/firewallexception.md) 
* [FormatFile (Util extension)](../util/formatfile.md) 
* [FormatsFile (Powershell extension)](../powershell/formatsfile.md) 
* [NativeImage (Netfx extension)](../netfx/nativeimage.md) 
* [ODBCDriver](odbcdriver.md) 
* [ODBCTranslator](odbctranslator.md) 
* [PerfCounter (Util extension)](../util/perfcounter.md) 
* [PerfCounterManifest (Util extension)](../util/perfcountermanifest.md) 
* [Permission](permission.md) : Used to configure the ACLs for this file.
* [PermissionEx (Util extension)](../util/permissionex.md) 
* [Shortcut](shortcut.md) : Target of the shortcut will be set to this file.
* [SnapIn (Powershell extension)](../powershell/snapin.md) 
* [SymbolPath](symbolpath.md) 
* [TypeLib](typelib.md) 
* [TypesFile (Powershell extension)](../powershell/typesfile.md) 
* [VsixPackage (Vs extension)](../vs/vsixpackage.md) 

## Attributes
**Assembly** (enumeration)
  : Specifies if this File is a Win32 Assembly or .NET Assembly that needs to be installed into the Global Assembly Cache (GAC). If the value is '.net' or 'win32', this file must also be the key path of the Component. This attribute's value must be one of the following:
- *.net*: The file is a .NET Framework assembly.
- *no*: The file is not a .NET Framework or Win32 assembly. This is the default value.
- *win32*: The file is a Win32 assembly.

**AssemblyApplication** (String)
  : Specifies the file identifier of the application file. This assembly will be isolated to the same directory as the application file. If this attribute is absent, the assembly will be installed to the Global Assembly Cache (GAC). This attribute may only be specified if the Assembly attribute is set to '.net' or 'win32'.

**AssemblyManifest** (String)
  : Specifies the file identifier of the manifest file that describes this assembly. The manifest file should be in the same component as the assembly it describes. This attribute may only be specified if the Assembly attribute is set to '.net' or 'win32'.

**BindPath** (String)
  : A list of paths, separated by semicolons, that represent the paths to be searched to find the imported DLLs. The list is usually a list of properties, with each property enclosed inside square brackets. The value may be set to an empty string. Including this attribute will cause an entry to be generated for the file in the BindImage table.

**Checksum** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute should be set to "yes" for every executable file in the installation that has a valid checksum stored in the Portable Executable (PE) file header. Only those files that have this attribute set will be verified for valid checksum during a reinstall.

**CompanionFile** (String)
  : Set this attribute to make this file a companion child of another file. The installation state of a companion file depends not on its own file versioning information, but on the versioning of its companion parent. A file that is the key path for its component can not be a companion file (that means this attribute cannot be set if KeyPath="yes" for this file). The Version attribute cannot be set along with this attribute since companion files are not installed based on their own version.

**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Sets the file's source type compression. A setting of "yes"/"true", or "no"/"false" will override the setting in the Word Count Summary Property.

**DefaultLanguage** (String)
  : This is the default language of this file. The linker will replace this value from the value in the file if the suppress files option is not used.

**DefaultSize** (Integer)
  : This is the default size of this file. The linker will replace this value from the value in the file if the suppress files option is not used.

**DefaultVersion** (String)
  : This is the default version of this file. The linker will replace this value from the value in the file if the suppress files option is not used.

**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : The value of this attribute should correspond to the Id attribute of a Media element authored elsewhere. By creating this connection between a file and its media, you set the packaging options to the values specified in the Media element (values such as compression level, cab embedding, etc...). Specifying the DiskId attribute on the File element overrides the default DiskId attribute from the parent Component element. If no DiskId attribute is specified, the default is "1". This DiskId attribute is ignored when creating a merge module because merge modules do not have media.

**FontTitle** (String)
  : Causes an entry to be generated for the file in the Font table with the specified FontTitle. This attribute is intended to be used to register the file as a non-TrueType font.

**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to yes in order to have the file's hidden attribute set when it is installed on the target machine.

**Id** (String)
  : The unique identifier for this File element. If you omit Id, it defaults to the file name portion of the Source attribute, if specified. May be referenced as a Property by specifying [#value].

**KeyPath** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to yes in order to force this file to be the key path for the parent component.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : In prior versions of the WiX toolset, this attribute specified the short file name. This attribute's value may now be either a short or long file name. If a short file name is specified, the ShortName attribute may not be specified. Also, if this value is a long file name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short file name. However, if this name collides with another file or you wish to manually specify the short file name, then the ShortName attribute may be specified. Finally, if this attribute is omitted then its default value is the file name portion of the Source attribute, if one is specified, or the value of the Id attribute, if the Source attribute is omitted or doesn't contain a file name.

**PatchAllowIgnoreOnError** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to indicate that the patch is non-vital.

**PatchGroup** (Integer)
  : This attribute must be set for patch-added files. Each patch should be assigned a different patch group number. Patch groups numbers must be greater 0 and should be assigned consecutively. For example, the first patch should use PatchGroup='1', the second patch will have PatchGroup='2', etc...

**PatchIgnore** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Prevents the updating of the file that is in fact changed in the upgraded image relative to the target images.

**PatchWholeFile** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set if the entire file should be installed rather than creating a binary patch.

**ProcessorArchitecture** (enumeration)
  : Specifies the architecture for this assembly. This attribute should only be used on .NET Framework 2.0 or higher assemblies. This attribute's value must be one of the following:
- *msil*: The file is a .NET Framework assembly that is processor-neutral.
- *x86*: The file is a .NET Framework assembly for the x86 processor.
- *x64*: The file is a .NET Framework assembly for the x64 processor.
- *ia64*: The file is a .NET Framework assembly for the ia64 processor.

**ReadOnly** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to yes in order to have the file's read-only attribute set when it is installed on the target machine.

**SelfRegCost** (Integer)
  : The cost of registering the file in bytes. This must be a non-negative number. Including this attribute will cause an entry to be generated for the file in the SelfReg table.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short file name of the file in 8.3 format. This attribute should only be set if there is a conflict between generated short file names or the user wants to manually specify the short file name.

**Source** (String)
  : Specifies the path to the File in the build process. Overrides default source path set by parent directories and Name attribute. This attribute must be set if no source information can be gathered from parent directories. For more information, see Specifying source files.

**System** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to yes in order to have the file's system attribute set when it is installed on the target machine.

**TrueType** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Causes an entry to be generated for the file in the Font table with no FontTitle specified. This attribute is intended to be used to register the file as a TrueType font.

**Vital** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If a file is vital, then installation cannot proceed unless the file is successfully installed. The user will have no option to ignore an error installing this file. If an error occurs, they can merely retry to install the file or abort the installation. The default is "yes," unless the -sfdvital switch (candle.exe) or SuppressFileDefaultVital property (.wixproj) is used.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)