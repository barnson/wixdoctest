---
custom_edit_url: null
sidebar_position: 180
---
# ProductSearch element


## Windows Installer references
[Upgrade Table](https://docs.microsoft.com/en-us/windows/win32/msi/upgrade-table)

## Parents
[Property](property.md)

## Attributes
**ExcludeLanguages** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to detect all languages, excluding the languages listed in the Language attribute.

**IncludeMaximum** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to make the range of versions detected include the value specified in Maximum.

**IncludeMinimum** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "no" to make the range of versions detected exclude the value specified in Minimum. This attribute is "yes" by default.

**Language** (String)
  : Specifies the set of languages detected by FindRelatedProducts. Enter a list of numeric language identifiers (LANGID) separated by commas (,). Leave this value null to specify all languages. Set ExcludeLanguages to "yes" in order detect all languages, excluding the languages listed in this value.

**Maximum** (String)
  : Specifies the upper boundary of the range of product versions detected by FindRelatedProducts.

**Minimum** (String)
  : Specifies the lower bound on the range of product versions to be detected by FindRelatedProducts.

**UpgradeCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : This value specifies the upgrade code for the products that are to be detected by the FindRelatedProducts action.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)