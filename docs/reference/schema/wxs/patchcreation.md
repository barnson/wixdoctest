---
custom_edit_url: null
sidebar_position: 164
---
# PatchCreation element
The PatchCreation element is analogous to the main function in a C program. When linking, only one PatchCreation section can be given to the linker to produce a successful result. Using this element creates a pcp file.

## Parents
[Wix](wix.md)

## Children
* [Family](family.md) 
* [PatchInformation](patchinformation.md) 
* [PatchMetadata](patchmetadata.md) 
* [PatchProperty](patchproperty.md) 
* [PatchSequence](patchsequence.md) 
* [ReplacePatch](replacepatch.md) 
* [TargetProductCode](targetproductcode.md) 

## Remarks
<p>You can specify any valid Windows code by by integer like 1252, or by web name like Windows-1252. See [Code pages](reference/codepage.md) for more information.</p>


## Attributes
**AllowMajorVersionMismatches** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use this to set whether the major versions between the upgrade and target images match. See AllowProductVersionMajorMismatches for more information.

**AllowProductCodeMismatches** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use this to set whether the product code between the upgrade and target images match. See AllowProductCodeMismatches for more information.

**CleanWorkingFolder** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use this to set whether Patchwiz should clean the temp folder when finished. See DontRemoveTempFolderWhenFinished for more information.

**Codepage** (String)
  : The code page integer value or web name for the resulting PCP. See remarks for more information.

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : PatchCreation identifier; this is the primary key for identifying patches.

**OutputPath** (String)
  : The full path, including file name, of the patch package file that is to be generated. See PatchOutputPath for more information.

**SourceList** (String)
  : Used to locate the .msp file for the patch if the cached copy is unavailable. See PatchSourceList for more information.

**SymbolFlags** (xs:int)
  : An 8-digit hex integer representing the combination of patch symbol usage flags to use when creating a binary file patch. See ApiPatchingSymbolFlags for more information.

**WholeFilesOnly** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use this to set whether changing files should be included in their entirety. See IncludeWholeFilesOnly for more information.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)