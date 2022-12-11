---
custom_edit_url: null
sidebar_position: 12
---
# ComPlusPartitionUser element (Complus extension)
Represents a default partition definition for a user. When the parent component of this element is installed, the default partition of the user will be set to the referenced partition.

## Parents
[Component](../wxs/component.md), [ComPlusPartition](compluspartition.md)

## Attributes
**Id** (String, required)
  : Identifier for the element.

**Partition** (String)
  : The id of a ComPlusPartition element representing the partition that will be the default partition for the user.

**User** (String, required)
  : Foreign key into the User table.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)