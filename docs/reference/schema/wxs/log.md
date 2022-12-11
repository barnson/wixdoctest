---
custom_edit_url: null
sidebar_position: 132
---
# Log element
Overrides the default log settings for a bundle.

## Parents
[Bundle](bundle.md)

## Attributes
**Disable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Disables the default logging in the Bundle. The end user can still generate a log file by specifying the "-l" command-line argument when installing the Bundle.

**Extension** (String)
  : The extension to use for the log. The default is ".log".

**PathVariable** (String)
  : Name of a Variable that will hold the path to the log file. An empty value will cause the variable to not be set. The default is "WixBundleLog".

**Prefix** (String)
  : File name and optionally a relative path to use as the prefix for the log file. The default is to use the Bundle/@Name or, if Bundle/@Name is not specified, the value "Setup".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)