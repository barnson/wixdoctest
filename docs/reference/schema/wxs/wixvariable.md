---
custom_edit_url: null
sidebar_position: 290
---
# WixVariable element
This element exposes advanced WiX functionality. Use this element to declare WiX variables from directly within your authoring. WiX variables are not resolved until the final msi/msm/pcp file is actually generated. WiX variables do not persist into the msi/msm/pcp file, so they cannot be used when an MSI file is being installed; it's a WiX-only concept.

## Parents
[Bundle](bundle.md), [Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Attributes
**Id** (String, required)
  : The name of the variable.

**Overridable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' in order to make the variable's value overridable either by another WixVariable entry or via the command-line option -d_name_=_value_; for light.exe. If the same variable is declared overridable in multiple places it will cause an error (since WiX won't know which value is correct). The default value is 'no'.

**Value** (String, required)
  : The value of the variable. The value cannot be an empty string because that would make it possible to accidentally set a column to null.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)