---
custom_edit_url: null
sidebar_position: 7
---
# ComPlusGroupInPartitionRole element (Complus extension)
This element represents a security group membership in a partition role. When the parent component of this element is installed, the security group will be added to the associated partition role.

## Parents
[Component](../wxs/component.md), [ComPlusPartitionRole](compluspartitionrole.md)

## Attributes
**Group** (String, required)
  : Foreign key into the Group table.

**Id** (String, required)
  : Identifier for the element.

**PartitionRole** (String)
  : The id of a ComPlusPartitionRole element representing the partition the user should be added to.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)