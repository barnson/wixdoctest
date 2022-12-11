---
custom_edit_url: null
sidebar_position: 187
---
# Provides element
Describes the information for this product or feature that serves as a dependency of other products or features.

## Parents
[MsiPackage](msipackage.md), [MspPackage](msppackage.md), [MsuPackage](msupackage.md), [ExePackage](exepackage.md), [BundlePackage](bundlepackage.md), [Component](component.md)

## Children
* [Requires](requires.md) 
* [RequiresRef](requiresref.md) 

## Remarks
<p>
  This element is required for any product, feature, or bundle that will use the Dependency feature to properly reference count
  other products or features. It should be authored into a component that is always installed and removed with the
  product or features that contain it. This guarantees that product dependencies are not removed before those products that
  depend on them.
</p>
<p>
  The @Key attribute should identify a version range for your product that you guarantee will be backward compatible.
  This key is designed to persist throughout compatible upgrades so that dependent products do not have to be reinstalled
  and will not prevent your product from being upgraded. If this attribute is not authored, the value is the ProductCode
  and will not automatically support upgrades.
</p>
<p>
  By default this uses the Package/@ProductCode attribute value, which may be automatically generated.
</p>


## Attributes
**DisplayName** (String)
  : Optional display name of the package. For MSI packages, the ProductName will be used by default.

**Id** (String)
  : Dependency provider identity. If this attribute is not specified, an identifier will be generated automatically.

**Key** (String)
  : Optional unique registry key name that identifies a product version range on which other products can depend. This attribute is required in package authoring, but optional for components.

**Version** ([VersionType](versiontype.md 'Values of this type will look like: "x.x.x.x" where x is an integer from 0 to 65534.'))
  : The version of the package. For MSI packages, the ProductVersion will be used by default and this attribute should not be specified.

**Check** (wxs:YesNoTypeUnion)
  : When set to "yes", adds a custom action to prompt the user when dependencies are still on the computer. The default is "no".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)