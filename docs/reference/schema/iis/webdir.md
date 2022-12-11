---
custom_edit_url: null
sidebar_position: 10
---
# WebDir element (Iis extension)
Defines a subdirectory within an IIS web site. When this element is a child of WebSite, the web directory is defined within that web site. Otherwise the web directory must reference a WebSite element via the WebSite attribute.

## Parents
[Component](../wxs/component.md), [WebSite](website.md)

## Children
* [WebApplication](webapplication.md) (no more than 1) 
* [WebDirProperties](webdirproperties.md) (no more than 1) 

## Attributes
**DirProperties** (String)
  : References the Id attribute for a WebDirProperties element that specifies the security and access properties for this web directory. This attribute may not be specified if a WebDirProperties element is directly nested in this element.

**Id** (String)
  : Identifier for the web application. If the Id is not specified, it will be generated.

**Path** (String, required)
  : Specifies the name of this web directory.

**WebApplication** (String)
  : References the Id attribute for a WebApplication element in which this directory belongs.

**WebSite** (String)
  : References the Id attribute for a WebSite element in which this directory belongs. Required when this element is not a child of a WebSite element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)