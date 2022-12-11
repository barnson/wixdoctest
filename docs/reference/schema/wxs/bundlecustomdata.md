---
custom_edit_url: null
sidebar_position: 23
---
# BundleCustomData element
Defines a custom XML element for use in a bundle data manifest.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Children
* [BundleAttributeDefinition](bundleattributedefinition.md) 
* [BundleElement](bundleelement.md) 

## Attributes
**ExtensionId** (String)
  : Identifier for the bundle extension. Required when Type is BundleExtension, must not be specified otherwise.

**Id** (String, required)
  : Identifier for the custom table. Also used as the name of the XML element.

**Type** (enumeration)
  : Indicates the custom data is transformed into the bootstrapper application data manifest or the bundle extension data manifest. Defaults to BundleExtension if ExtensionId is specified, otherwise BootstrapperApplication. This attribute's value must be one of the following:
- *BootstrapperApplication*
- *BundleExtension*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)