---
custom_edit_url: null
sidebar_position: 46
---
# Container element
Representation of a file that contains one or more files.

## Parents
[Bundle](bundle.md), [Fragment](fragment.md)

## Children
* [PackageGroupRef](packagegroupref.md) 

## Attributes
**DownloadUrl** (String)
  : The URL to use to download the container. This attribute is only valid when the container is detached. The following substitutions are supported:  {0} is always null. {1} is replaced by the container Id. {2} is replaced by the container file name.

**Id** (String)
  : The unique identifier for the container. If this attribute is not specified the Name attribute will be used.

**Name** (String)
  : The file name for this container. A relative path may be provided to place the container in a sub-folder of the bundle.

**Type** (enumeration)
  : Indicates whether the container is "attached" to the bundle executable or placed external to the bundle extecutable as "detached". If this attribute is not specified, the default is to create a detached container. This attribute's value must be one of the following:
- *attached*
- *detached*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)