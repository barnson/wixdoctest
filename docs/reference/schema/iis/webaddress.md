---
custom_edit_url: null
sidebar_position: 6
---
# WebAddress element (Iis extension)
WebAddress for WebSite

## Parents
[WebSite](website.md)

## Attributes
**Header** (String)
  : 

**Id** (String)
  : Identifier for the web application. If the Id is not specified, it will be generated.

**IP** (String)
  : The IP address to locate an existing WebSite or create a new WebSite. When the WebAddress is part of a WebSite element used to locate an existing web site the following rules are used:  When this attribute is not specified only the "All Unassigned" IP address will be located. When this attribute is explicitly specified only the specified IP address will be located. When this attribute has the value "*" then any IP address including the "All Unassigned" IP address will be located   When the WebAddress is part of a WebSite element used to create a new web site the following rules are used:   When this attribute is not specified or the value is "*" the "All Unassigned" IP address will be used. When this attribute is explicitly specified the IP address will use that value.   The IP attribute can contain a formatted string that is processed at install time to insert the values of properties using [PropertyName] syntax.

**Port** (String, required)
  : 

**Secure** (wxs:YesNoTypeUnion)
  : Determines if this address represents a secure binding.  The default is 'no'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)