---
custom_edit_url: null
sidebar_position: 69
---
# Directory element
Directory layout for the product. Also specifies the mappings between source and target directories.

## Windows Installer references
[Directory Table](https://docs.microsoft.com/en-us/windows/win32/msi/directory-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [Directory](directory.md), [DirectoryRef](directoryref.md), [StandardDirectory](standarddirectory.md)

## Children
* [Component](component.md) 
* [Directory](directory.md) 
* [Merge](merge.md) 
* [SymbolPath](symbolpath.md) 

## Attributes
**ComponentGuidGenerationSeed** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : The Component Guid Generation Seed is a guid that must be used when a Component with the generate guid directive ("*") is not rooted in a standard Windows Installer directory (for example, ProgramFilesFolder or CommonFilesFolder). It is recommended that this attribute be avoided and that developers install their Components under standard directories with unique names instead (for example, "ProgramFilesFolder\Company Name Product Name Version"). It is important to note that once a directory is assigned a Component Guid Generation Seed the value must not change until (and must be changed when) the path to that directory, including itself and all parent directories, changes.

**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : Sets the default disk identifier for the files contained in this directory. This attribute's value may be overridden by a child Component, Directory, Merge or File element. See the File or Merge elements' DiskId attribute for more information.

**FileSource** (String)
  : Used to set the file system source for this directory's child elements. For more information, see Specifying source files.

**Id** (String, required)
  : This value is the unique identifier of the directory entry.

**Name** (String)
  : The name of the directory.  Do not specify this attribute if this directory represents the same directory as the parent (see the Windows Installer SDK's Directory table topic for more information about the "." operator).  This attribute's value may either a short or long directory name. If a short directory name is specified, the ShortName attribute may not be specified. If this value is a long directory name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short directory name. However, if this name collides with another directory or you wish to manually specify the short directory name, then the ShortName attribute may be specified.  This Name attribute may also define multiple directories using the inline directory syntax. For example, "ProgramFilesFolder:\My Company\My Product\bin" would create a reference to a Directory element with Id="ProgramFilesFolder" then create directories named "My Company" then "My Product" then "bin" nested beneath each other. This syntax is a shortcut to defining each directory in an individual Directory element.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short name of the directory in 8.3 format. This attribute should only be set if there is a conflict between generated short directory names or the user wants to manually specify the short directory name.

**ShortSourceName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short name of the directory on the source media in 8.3 format. This attribute should only be set if there is a conflict between generated short directory names or the user wants to manually specify the short source directory name.

**SourceName** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The name of the directory on the source media. If this attribute is not specified, Windows Installer will default to the Name attribute.  In prior versions of the WiX toolset, this attribute specified the short source directory name. This attribute's value may now be either a short or long directory name. If a short directory name is specified, the ShortSourceName attribute may not be specified. If a long directory name is specified, the LongSource attribute may not be specified. Also, if this value is a long directory name, the ShortSourceName attribute may be omitted to allow WiX to attempt to generate a unique short directory name. However, if this name collides with another directory or you wish to manually specify the short directory name, then the ShortSourceName attribute may be specified.


## See also
[DirectoryRef](directoryref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)