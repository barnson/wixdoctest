---
custom_edit_url: null
sidebar_position: 205
---
# RegistrySearch element
Searches for file, directory or registry key and assigns to value of parent Property

## Windows Installer references
[RegLocator Table](https://docs.microsoft.com/en-us/windows/win32/msi/reglocator-table), [Signature Table](https://docs.microsoft.com/en-us/windows/win32/msi/signature-table)

## Parents
[ComplianceCheck](compliancecheck.md), [Property](property.md)

## Children
* [DirectorySearch](directorysearch.md) (no more than 1) 
* [DirectorySearchRef](directorysearchref.md) (no more than 1) 
* [FileSearch](filesearch.md) (no more than 1) 
* [FileSearchRef](filesearchref.md) (no more than 1) 

## Remarks
<p>
              When the Type attribute value is 'directory' the registry value must specify the path to a directory excluding the file name.
              When the Type attribute value is 'file' the registry value must specify the path to a file including the file name;
              however, if there is no child FileSearch element the parent directory of the file is returned. The FileSearch element requires
              that you author the name of the file you are searching for. If you do not know the file name
              you must set the Type attribute to 'raw' to return the full file path including the file name.
          </p>


## Attributes
**Bitness** ([BitnessTypeUnion](bitnesstype.md 'Values of this type will be "default", "always32" or "always64".'))
  : Overrides the default registry to search. The value `always64` will force the search to look in the 64-bit registry even when building for 32-bit. Simliarly, the value `always32` will force the search to look in the 32-bit registry even when building for 64-bit. The default value is `default` where the search will look in the same registry as the bitness of the package.

**Id** (String, required)
  : Signature to be used for the file, directory or registry key being searched for.

**Key** (String, required)
  : Key for the registry value.

**Name** (String)
  : Registry value name. If this value is null, then the value from the key's unnamed or default value, if any, is retrieved.

**Root** (enumeration, required)
  : Root key for the registry value. This attribute's value must be one of the following:
- *HKCR*: HKEY_CLASSES_ROOT
- *HKCU*: HKEY_CURRENT_USER
- *HKLM*: HKEY_LOCAL_MACHINE
- *HKU*: HKEY_USERS

**Type** (enumeration, required)
  : The value must be 'file' if the child is a FileSearch element, and must be 'directory' if child is a DirectorySearch element. This attribute's value must be one of the following:
- *directory*: The registry value contains the path to a directory.
- *file*: The registry value contains the path to a file. To return the full file path you must add a FileSearch element as a child of this element; otherwise, the parent directory of the file path is returned.
- *raw*: Sets the raw value from the registry value. Please note that this value will contain a prefix as follows:DWORDStarts with '#' optionally followed by '+' or '-'.REG_BINARYStarts with '#x' and the installer converts and saves each hexadecimal digit (nibble) as an ASCII character prefixed by '#x'.REG_EXPAND_SZStarts with '#%'.REG_MULTI_SZStarts with '[~]' and ends with '[~]'.REG_SZNo prefix, but if the first character of the registry value is '#', the installer escapes the character by prefixing it with another '#'.


## See also
[ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)