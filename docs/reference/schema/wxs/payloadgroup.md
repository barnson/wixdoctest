---
custom_edit_url: null
sidebar_position: 175
---
# PayloadGroup element
Describes a payload group to a bootstrapper. PayloadGroups referenced from within a Bundle are tied to the Bundle. PayloadGroups referenced from a Fragment are tied to the context of whatever references them such as an ExePackage or MsiPackage. It is possible to share a PayloadGroup between multiple Packages and/or a Bundle by creating multiple references to it.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Children
* [BundlePackagePayload](bundlepackagepayload.md) 
* [ExePackagePayload](exepackagepayload.md) 
* [MsiPackagePayload](msipackagepayload.md) 
* [MspPackagePayload](msppackagepayload.md) 
* [MsuPackagePayload](msupackagepayload.md) 
* [Payload](payload.md) 
* [PayloadGroupRef](payloadgroupref.md) 

## Attributes
**Id** (String, required)
  : Identifier for payload group.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)