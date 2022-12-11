---
custom_edit_url: null
sidebar_position: 226
---
# Requires element
Describes a dependency on a provider for the current component or package.

## Parents
[Bundle](bundle.md), [Package](package.md), [Module](module.md), [Fragment](fragment.md), [Provides](provides.md)

## Remarks
<p>
  This element declares a dependency on any product that uses the Provides element. If that product is uninstalled
  before a product that requires it, the uninstall will err or warn the user that other products are installed
  which depend on that product. This behavior can be modified by changing the attribute values on the Requires element.
</p>
<p>
  If you do not nest this element under a Provides element, you must specify the @Id attribute
  so that it can be referenced by a RequiresRef element nested under a Provides element.
</p>


## Attributes
**Id** (String)
  : Dependency requirement identity. If this attribute is not specified, an identifier will be generated automatically. If this element is not authored under a Provides element, this attribute is required.

**IncludeMaximum** (enumeration)
  : Set to "yes" to make the range of dependency provider versions required include the value specified in Maximum. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**IncludeMinimum** (enumeration)
  : Set to "yes" to make the range of dependency provider versions required include the value specified in Minimum. This attribute's value must be one of the following:
- *no*
- *false*
- *yes*
- *true*

**Maximum** ([VersionType](versiontype.md 'Values of this type will look like: "x.x.x.x" where x is an integer from 0 to 65534.'))
  : The maximum version of the dependency provider required to be installed. The default is unbound.

**Minimum** ([VersionType](versiontype.md 'Values of this type will look like: "x.x.x.x" where x is an integer from 0 to 65534.'))
  : The minimum version of the dependency provider required to be installed. The default is unbound.

**ProviderKey** (String, required)
  : The unique registry key name for the dependency provider to require during installation of this product.

**Enforce** (wxs:YesNoTypeUnion)
  : When set to "yes", adds a custom action to prompt the user when dependencies are missing from the computer. The default is "no".


## See also
[RequiresRef](requiresref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)