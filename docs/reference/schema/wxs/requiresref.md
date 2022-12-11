---
custom_edit_url: null
sidebar_position: 227
---
# RequiresRef element
References existing authoring for a dependency on a provider for the current component or package.

## Parents
[Provides](provides.md)

## Remarks
<p>
  This element references a dependency on any product that uses the Provides element. If that product is uninstalled
  before a product that requires it, the uninstall will err or warn the user that other products are installed
  which depend on that product. This behavior can be modified by changing the attribute values on the Requires element.
</p>


## Attributes
**Id** (String, required)
  : The identifier of the Requires element to reference.

**Enforce** (wxs:YesNoTypeUnion)
  : When set to "yes", adds a custom action to prompt the user when dependencies are missing from the computer. The default is "no".


## See also
[Requires](requires.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)