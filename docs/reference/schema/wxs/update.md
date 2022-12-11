---
custom_edit_url: null
sidebar_position: 280
---
# Update element
Defines the update for a Bundle.

## Parents
[Bundle](bundle.md)

## Attributes
**Location** (String, required)
  : The absolute path or URL to check for an update bundle. Currently the engine provides this value in the IBootstrapperApplication::OnDetectUpdateBegin() and otherwise ignores the value. In the future the engine will be able to acquire an update bundle from the location and determine if it is newer than the current executing bundle.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)