---
custom_edit_url: null
sidebar_position: 15
---
# WebProperty element (Iis extension)
IIS Properties

## Parents
[Component](../wxs/component.md)

## Remarks
Here is an explanation of the acceptable values for each property and their meaning:
<ul>
  <li>
    For the Ids IIs5IsolationMode and LogInUTF8, no value should be specified since
    the presence of this property indicates that the setting should be set.
  </li>
  <li>
    For the MaxGlobalBandwidth Id, the value should be specified in kilobytes.  The
    value should be a base 10 number.
  </li>
  <li>
    ETagChangeNumber sets the machine-specific portion of ETag as a number. This value,
    when synchronized across servers in a web farm, allows the web farm to return an
    identical ETag for a given resource regardless of the server that handled the
    request.  The value should be a base 10 number.
  </li>
</ul>


## Attributes
**Id** (enumeration, required)
  :  This attribute's value must be one of the following:
- *ETagChangeNumber*
- *IIs5IsolationMode*
- *MaxGlobalBandwidth*
- *LogInUTF8*

**Value** (String)
  : The value to be used for the WebProperty specified in the Id attribute.  See the remarks section for information on acceptable values for each Id.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)