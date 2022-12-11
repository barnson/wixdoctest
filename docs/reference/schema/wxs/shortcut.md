---
custom_edit_url: null
sidebar_position: 249
---
# Shortcut element
Shortcut, default target is parent File, CreateFolder, or Component's Directory

## Windows Installer references
[Shortcut Table](https://docs.microsoft.com/en-us/windows/win32/msi/shortcut-table)

## Parents
[File](file.md), [CreateFolder](createfolder.md), [Component](component.md)

## Children
* [Icon](icon.md) 
* [ShortcutProperty](shortcutproperty.md) 

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies if the shortcut should be advertised or not. Note that advertised shortcuts always point at a particular application, identified by a ProductCode, and should not be shared between applications. Advertised shortcuts only work for the most recently installed application, and are removed when that application is removed. The default value is 'no'.

**Arguments** (String)
  : The command-line arguments for the shortcut. Note that the resolution of properties in the Arguments field is limited. A property formatted as [Property] in this field can only be resolved if the property already has the intended value when the component owning the shortcut is installed. For example, for the argument "[#MyDoc.doc]" to resolve to the correct value, the same process must be installing the file MyDoc.doc and the component that owns the shortcut.

**Description** (String)
  : The localizable description for the shortcut.

**DescriptionResourceDll** (String)
  : The Formatted string providing the full path to the language neutral file containing the MUI Manifest. Generally authored using [#filekey] form. When this attribute is specified, the DescriptionResourceId attribute must also be provided.  This attribute is only used on Windows Vista and above. If this attribute is not specified and the install is running on Vista and above, the value in the Name attribute is used. If this attribute is provided and the install is running on Vista and above, the value in the Name attribute is ignored.

**DescriptionResourceId** (Integer)
  : The description name index for the shortcut. This must be a non-negative number. When this attribute is specified, the DescriptionResourceDll attribute must also be populated.  This attribute is only used on Windows Vista and above. If this attribute is not specified and the install is running on Vista and above, the value in the Name attribute is used. If this attribute is populated and the install is running on Vista and above, the value in the Name attribute is ignored.

**Directory** (String)
  : Identifier reference to Directory element where shortcut is to be created. When nested under a Component element, this attribute's value will default to the parent directory. Otherwise, this attribute is required.

**DisplayResourceDll** (String)
  : The Formatted string providing the full path to the language neutral file containing the MUI Manifest. Generally authored using [#filekey] form. When this attribute is specified, the DisplayResourceId attribute must also be provided.  This attribute is only used on Windows Vista and above. If this attribute is not populated and the install is running on Vista and above, the value in the Name attribute is used. If this attribute is populated and the install is running on Vista and above, the value in the Name attribute is ignored.

**DisplayResourceId** (Integer)
  : The display name index for the shortcut. This must be a non-negative number. When this attribute is specified, the DisplayResourceDll attribute must also be provided.  This attribute is only used on Windows Vista and above. If this attribute is not specified and the install is running on Vista and above, the value in the Name attribute is used. If this attribute is specified and the install is running on Vista and above, the value in the Name attribute is ignored.

**Hotkey** (Integer)
  : The hotkey for the shortcut. The low-order byte contains the virtual-key code for the key, and the high-order byte contains modifier flags. This must be a non-negative number. Authors of installation packages are generally recommend not to set this option, because this can add duplicate hotkeys to a users desktop. In addition, the practice of assigning hotkeys to shortcuts can be problematic for users using hotkeys for accessibility.

**Icon** (String)
  : Identifier reference to Icon element. The Icon identifier should have the same extension as the file that it points at. For example, a shortcut to an executable (e.g. "my.exe") should reference an Icon with identifier like "MyIcon.exe"

**IconIndex** (Integer)
  : Identifier reference to Icon element.

**Id** (String, required)
  : Unique identifier for the shortcut. This value will serve as the primary key for the row.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'), required)
  : In prior versions of the WiX toolset, this attribute specified the short name. This attribute's value may now be either a short or long name. If a short name is specified, the ShortName attribute may not be specified. Also, if this value is a long name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short name. However, if this name collides with another shortcut or you wish to manually specify the short name, then the ShortName attribute may be specified.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short name of the shortcut in 8.3 format. This attribute should only be set if there is a conflict between generated short names or the user wants to manually specify the short name.

**Show** (enumeration)
  :  This attribute's value must be one of the following:
- *normal*: The shortcut target will be displayed using the SW_SHOWNORMAL attribute.
- *minimized*: The shortcut target will be displayed using the SW_SHOWMINNOACTIVE attribute.
- *maximized*: The shortcut target will be displayed using the SW_SHOWMAXIMIZED attribute.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute where the shortcut will be installed.

**Target** (String)
  : This attribute can only be set if this Shortcut element is nested under a Component element. When nested under a Component element, this attribute's value will default to the parent directory. This attribute's value is the target for a non-advertised shortcut. This attribute is not valid for advertised shortcuts. If you specify this value, its value should be a property identifier enclosed by square brackets ([ ]), that is expanded into the file or a folder pointed to by the shortcut.

**WorkingDirectory** (String)
  : Directory identifier (or Property identifier that resolves to a directory) that resolves to the path of the working directory for the shortcut.

**WorkingSubdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the WorkingDirectory attribute for the shortcut's working directory.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)