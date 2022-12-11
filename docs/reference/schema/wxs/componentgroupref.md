---
custom_edit_url: null
sidebar_position: 41
---
# ComponentGroupRef element
Create a reference to a ComponentGroup in another Fragment.

## Parents
[Module](module.md), [ComponentGroup](componentgroup.md), [Feature](feature.md), [FeatureGroup](featuregroup.md), [FeatureRef](featureref.md)

## Attributes
**Id** (String, required)
  : The identifier of the ComponentGroup to reference.

**Primary** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to 'yes' in order to make the parent feature of this component the primary feature for this component. Components may belong to multiple features. By designating a feature as the primary feature of a component, you ensure that whenever a component is selected for install-on-demand (IOD), the primary feature will be the one to install it. This attribute should only be set if a component actually nests under multiple features. If a component nests under only one feature, that feature is the primary feature for the component. You cannot set more than one feature as the primary feature of a given component.


## See also
[ComponentGroup](componentgroup.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)