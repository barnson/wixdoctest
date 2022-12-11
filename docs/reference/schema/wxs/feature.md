---
custom_edit_url: null
sidebar_position: 91
---
# Feature element
A feature for the Feature table. Features are the smallest installable unit. See msi.chm for more detailed information on the myriad installation options for a feature.

## Windows Installer references
[Feature Table](https://docs.microsoft.com/en-us/windows/win32/msi/feature-table)

## Parents
[Package](package.md), [Fragment](fragment.md), [Feature](feature.md), [FeatureGroup](featuregroup.md), [FeatureRef](featureref.md)

## Children
* [Component](component.md) 
* [ComponentGroupRef](componentgroupref.md) 
* [ComponentRef](componentref.md) 
* [Feature](feature.md) 
* [FeatureGroupRef](featuregroupref.md) 
* [FeatureRef](featureref.md) 
* [Level](level.md) 
* [MergeRef](mergeref.md) 

## Attributes
**AllowAbsent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute determines if a user will have the option to set a feature to absent in the user interface.

**AllowAdvertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute determines the possible advertise states for this feature. The default is 'yes'.

**ConfigurableDirectory** (String)
  : Specify the Id of a Directory that can be configured by the user at installation time. This identifier must be a public property and therefore completely uppercase.

**Description** (String)
  : Longer string of text describing the feature. This localizable string is displayed by the Text Control of the Selection Dialog.

**Display** (String)
  : Determines the initial display of this feature in the feature tree. This attribute's value should be one of the following:  collapse Initially shows the feature collapsed. This is the default value.expandInitially shows the feature expanded.hiddenPrevents the feature from displaying in the user interface.(an explicit integer value) For advanced users only, it is possible to directly set the integer value of the display value that will appear in the Feature row.

**Id** (String, required)
  : Unique identifier of the feature. The id must be shorter than 38 characters.

**InstallDefault** (enumeration)
  : This attribute determines the default install/run location of a feature. This attribute cannot be specified if the value of the FollowParent attribute is 'yes' since that would ask the installer to force this feature to follow the parent installation state and simultaneously favor a particular installation state just for this feature. This attribute's value must be one of the following:
- *followParent*: Forces the feature to follow the same installation state as its parent feature.
- *local*: Favors installing this feature locally by setting the msidbFeatureAttributesFavorLocal attribute.
- *source*: Favors running this feature from source by setting the msidbFeatureAttributesFavorSource attribute.

**Level** (Integer)
  : Sets the install level of this feature. A value of 0 will disable the feature. Processing the Condition Table can modify the level value (this is set via the Condition child element). The default value is "1".

**Title** (String)
  : Short string of text identifying the feature. This string is listed as an item by the SelectionTree control of the Selection Dialog.

**TypicalDefault** (enumeration)
  : This attribute determines the default advertise state of the feature. This attribute's value must be one of the following:
- *advertise*: Sets the feature to be advertised by setting the msidbFeatureAttributesFavorAdvertise attribute. This value cannot be set if the value of the AllowAdvertise attribute is 'no' since that would ask the installer to disallow the advertised state for this feature while at the same time favoring it.
- *install*: Sets the feature to the default non-advertised installation option.


## See also
[FeatureRef](featureref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)