---
custom_edit_url: null
sidebar_position: 94
---
# FeatureRef element
Create a reference to a Feature element in another Fragment.

## Parents
[Package](package.md), [Fragment](fragment.md), [PatchFamily](patchfamily.md), [Feature](feature.md), [FeatureGroup](featuregroup.md), [FeatureRef](featureref.md)

## Children
* [Component](component.md) 
* [ComponentGroupRef](componentgroupref.md) 
* [ComponentRef](componentref.md) 
* [Feature](feature.md) 
* [FeatureGroup](featuregroup.md) 
* [FeatureGroupRef](featuregroupref.md) 
* [FeatureRef](featureref.md) 
* [MergeRef](mergeref.md) 

## Attributes
**Id** (String, required)
  : The identifier of the Feature element to reference.

**IgnoreParent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Normally feature references that are nested under a parent element create a connection to that parent. This behavior is undesirable when trying to simply reference a Feature in a different Fragment. Specify 'yes' to have this feature reference not create a connection to its parent. The default is 'no'.


## See also
[Feature](feature.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)