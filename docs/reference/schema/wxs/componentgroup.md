---
custom_edit_url: null
sidebar_position: 40
---
# ComponentGroup element
Groups together multiple components to be used in other locations.

## Parents
[Package](package.md), [Fragment](fragment.md)

## Children
* [Component](component.md) 
* [ComponentGroupRef](componentgroupref.md) 
* [ComponentRef](componentref.md) 

## Attributes
**Directory** (String)
  : Sets the default directory identifier for child Component elements.

**Id** (String, required)
  : Identifier for the ComponentGroup.

**Source** (String)
  : Used to set the default file system source for child Component elements. For more information, see Specifying source files.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute or parent Directory reference where the contained Components will be installed.


## See also
[ComponentGroupRef](componentgroupref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)