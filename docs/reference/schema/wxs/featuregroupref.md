---
custom_edit_url: null
sidebar_position: 93
---
# FeatureGroupRef element
Create a reference to a FeatureGroup in another Fragment.

## Parents
[Package](package.md), [Feature](feature.md), [FeatureGroup](featuregroup.md), [FeatureRef](featureref.md)

## Attributes
**Id** (String, required)
  : The identifier of the FeatureGroup to reference.

**IgnoreParent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Normally feature group references that end up nested under a parent element create a connection to that parent. This behavior is undesirable when trying to simply reference to a FeatureGroup in a different Fragment. Specify 'yes' to have this feature group reference not create a connection to its parent. The default is 'no'.

**Primary** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to 'yes' in order to make the parent feature of this group the primary feature for any components and merges contained in the group. Features may belong to multiple features. By designating a feature as the primary feature of a component or merge, you ensure that whenever a component is selected for install-on-demand (IOD), the primary feature will be the one to install it. This attribute should only be set if a component actually nests under multiple features. If a component nests under only one feature, that feature is the primary feature for the component. You cannot set more than one feature as the primary feature of a given component.


## See also
[FeatureGroup](featuregroup.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)