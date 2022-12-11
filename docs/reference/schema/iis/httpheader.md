---
custom_edit_url: null
sidebar_position: 3
---
# HttpHeader element (Iis extension)
Custom HTTP Header definition for IIS resources such as WebSite and WebVirtualDir.

## Parents
[WebVirtualDir](webvirtualdir.md), [WebSite](website.md)

## Attributes
**Id** (String)
  : Primary key for custom HTTP Header entry. This will default to the Name attribute.

**Name** (String, required)
  : Name of the custom HTTP Header.

**Value** (String)
  : Value for the custom HTTP Header. This attribute can contain a formatted string that is processed at install time to insert the values of properties using [PropertyName] syntax. Also supported are environment variables, file installation paths, and component installation directories; see Formatted for details.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)