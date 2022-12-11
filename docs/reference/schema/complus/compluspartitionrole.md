---
custom_edit_url: null
sidebar_position: 11
---
# ComPlusPartitionRole element (Complus extension)
Defines a COM+ partition role. Partition roles can not be created; this element can only be used as a locater to reference an existing role.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md), [ComPlusPartition](compluspartition.md)

## Children
* [ComPlusGroupInPartitionRole](complusgroupinpartitionrole.md) 
* [ComPlusUserInPartitionRole](complususerinpartitionrole.md) 

## Attributes
**Id** (String, required)
  : Identifier for the element.

**Name** (String, required)
  : Name of the partition role.

**Partition** (String)
  : The id of a ComPlusPartition element representing the partition the role belongs to.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)