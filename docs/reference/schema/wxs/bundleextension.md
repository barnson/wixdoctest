---
custom_edit_url: null
sidebar_position: 26
---
# BundleExtension element
An extension to the Burn engine. Currently requires a WiX compiler extension to do anything useful.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Children
* [Payload](payload.md) 
* [PayloadGroupRef](payloadgroupref.md) 

## Attributes
**Id** (String)
  : The identifier of the BundleExtension element. Only required if you want to reference this element using a BundleExtensionRef element.

**Name** (String)
  : The relative destination path and file name for the bundle extension DLL. The default is the source file name. Use this attribute to rename the bundle extension DLL or extract it into a subfolder. At a minimum, the Name or SourceFile attribute must be specified. This must be a relative path ('\foo' or 'C:\foo' is not allowed).

**SourceFile** (String)
  : The DLL with the bundle extension entry function. The default value is the Name attribute, if provided. At a minimum, the SourceFile or Name attribute must be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)