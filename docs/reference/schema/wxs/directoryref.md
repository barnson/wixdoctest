---
custom_edit_url: null
sidebar_position: 70
---
# DirectoryRef element
Create a reference to a Directory element in another Fragment.

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [PatchFamily](patchfamily.md)

## Children
* [Component](component.md) 
* [Directory](directory.md) 
* [Merge](merge.md) 

## Attributes
**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : Sets the default disk identifier for the files contained in this directory. This attribute's value may be overridden by a child Component, Directory, Merge or File element. See the File or Merge elements' DiskId attribute for more information.

**FileSource** (String)
  : Used to set the file system source for this DirectoryRef's child elements. For more information, see Specifying source files.

**Id** (String, required)
  : The identifier of the Directory element to reference.


## See also
[Directory](directory.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)