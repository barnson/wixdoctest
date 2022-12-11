---
custom_edit_url: null
sidebar_position: 18
---
# WebVirtualDir element (Iis extension)
Defines an IIS virtual directory. When this element is a child of WebSite element, the virtual directory is defined within that web site. Otherwise this virtual directory must reference a WebSite element via the WebSite attribute

## Parents
[Component](../wxs/component.md), [WebVirtualDir](webvirtualdir.md), [WebSite](website.md)

## Children
* [HttpHeader](httpheader.md) 
* [MimeMap](mimemap.md) 
* [WebApplication](webapplication.md) (no more than 1) 
* [WebDirProperties](webdirproperties.md) (no more than 1) 
* [WebError](weberror.md) 
* [WebVirtualDir](webvirtualdir.md) 

## Attributes
**Alias** (String, required)
  : Sets the application name, which is the URL relative path used to access this virtual directory

**Directory** (String, required)
  : References the Id attribute for a Directory element that points to the content for this virtual directory.

**DirProperties** (String)
  : References the Id attribute for a WebDirProperties element that specifies the security and access properties for this virtual directory. This attribute may not be specified if a WebDirProperties element is directly nested in this element.

**Id** (String)
  : Identifier for the web application. If the Id is not specified, it will be generated.

**WebApplication** (String)
  : References the Id attribute for a WebApplication element that specifies web application settings for this virtual directory.  If a WebApplication child is not specified, the virtual directory does not host web applications.

**WebSite** (String)
  : References the Id attribute for a WebSite in which this virtual directory belongs. Required when this element is not a child of WebSite element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)