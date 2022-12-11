---
custom_edit_url: null
sidebar_position: 10
---
# ComPlusPartition element (Complus extension)
Defines a COM+ partition. If this element is a child of a Component element, the partition will be created in association with this component. If the element is a child of any of the Fragment, Module, or Package elements it is considered to be a locater, referencing an existing partition.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Children
* [ComPlusApplication](complusapplication.md) 
* [ComPlusPartitionRole](compluspartitionrole.md) 
* [ComPlusPartitionUser](compluspartitionuser.md) 

## Attributes
**Changeable** (wxs:YesNoTypeUnion)
  : 

**Deleteable** (wxs:YesNoTypeUnion)
  : 

**Description** (String)
  : 

**Id** (String, required)
  : Identifier for the element.

**Name** (String)
  : Name of the partition. This attribute can be omitted if the element is a locater, and a value is provided for the PartitionId attribute.

**PartitionId** (String)
  : Id for the partition. This attribute can be omitted, in which case an id will be generated on install. If the element is a locater, this attribute can be omitted if a value is provided for the Name attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)