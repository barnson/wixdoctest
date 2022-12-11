---
custom_edit_url: null
sidebar_position: 134
---
# Media element
Media element describes a disk that makes up the source media for the installation.

## Windows Installer references
[Media Table](https://docs.microsoft.com/en-us/windows/win32/msi/media-table)

## Parents
[Package](package.md), [Fragment](fragment.md), [Patch](patch.md)

## Children
* [DigitalSignature](digitalsignature.md) 
* [PatchBaseline](patchbaseline.md) 
* [SymbolPath](symbolpath.md) 

## Attributes
**Cabinet** (String)
  : The name of the cabinet if some or all of the files stored on the media are in a cabinet file. If no cabinets are used, this attribute must not be set.

**CompressionLevel** ([CompressionLevelTypeUnion](compressionleveltype.md 'Indicates the compression level for a cabinet.'))
  : Indicates the compression level for the Media's cabinet. This attribute can only be used in conjunction with the Cabinet attribute. The default is 'mszip'.

**DiskPrompt** (String)
  : The disk name, which is usually the visible text printed on the disk. This localizable text is used to prompt the user when this disk needs to be inserted. This value will be used in the "[1]" of the DiskPrompt Property. Using this attribute will require you to define a DiskPrompt Property.

**EmbedCab** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Instructs the binder to embed the cabinet in the product if 'yes'. This attribute can only be specified in conjunction with the Cabinet attribute.

**Id** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'), required)
  : Disk identifier for Media table. This number must be equal to or greater than 1.

**Layout** (String)
  : This attribute specifies the root directory for the uncompressed files that are a part of this Media element. By default, the src will be the output directory for the final image. The default value ensures the binder generates an installable image. If a relative path is specified in the src attribute, the value will be appended to the image's output directory. If an absolute path is provided, that path will be used without modification. The latter two options are provided to ease the layout of an image onto multiple medias (CDs/DVDs).

**Source** (String)
  : Optional property that identifies the source of the embedded cabinet. If a cabinet is specified for a patch, this property should be defined and unique to each patch so that the embedded cabinet containing patched and new files can be located in the patch package. If the cabinet is not embedded - this is not typical - the cabinet can be found in the directory referenced in this column. If empty, the external cabinet must be located in the SourceDir directory.

**VolumeLabel** (String)
  : The label attributed to the volume. This is the volume label returned by the GetVolumeInformation function. If the SourceDir property refers to a removable (floppy or CD-ROM) volume, then this volume label is used to verify that the proper disk is in the drive before attempting to install files. The entry in this column must match the volume label of the physical media.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)