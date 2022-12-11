---
custom_edit_url: null
sidebar_position: 136
---
# Merge element
Merge directive to bring in a merge module that will be redirected to the parent directory.

## Parents
[Directory](directory.md), [DirectoryRef](directoryref.md), [StandardDirectory](standarddirectory.md)

## Children
* [ConfigurationData](configurationdata.md) 

## Attributes
**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : The value of this attribute should correspond to the Id attribute of a Media element authored elsewhere. By creating this connection between the merge module and Media element, you set the packaging options to the values specified in the Media element (values such as compression level, cab embedding, etc...).

**FileCompression** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies if the files in the merge module should be compressed.

**Id** (String, required)
  : The unique identifier for the Merge element in the source code. Referenced by the MergeRef/@Id.

**Language** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : Specifies the decimal LCID or localization token for the language to merge the Module in as.

**SourceFile** (String)
  : Path to the source location of the merge module.


## See also
[MergeRef](mergeref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)