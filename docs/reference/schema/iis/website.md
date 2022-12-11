---
custom_edit_url: null
sidebar_position: 17
---
# WebSite element (Iis extension)
IIs Web Site

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Children
* [CertificateRef](certificateref.md) 
* [HttpHeader](httpheader.md) 
* [MimeMap](mimemap.md) 
* [WebAddress](webaddress.md) (required, ) 
* [WebApplication](webapplication.md) (no more than 1) 
* [WebDir](webdir.md) 
* [WebDirProperties](webdirproperties.md) (no more than 1) 
* [WebError](weberror.md) 
* [WebFilter](webfilter.md) 
* [WebVirtualDir](webvirtualdir.md) 

## Remarks
<dl>
  <dd>Nesting WebSite under a Component element will result in a WebSite being installed to the machine as the package is installed.</dd>
  <dd>
    Nesting WebSite under Package, Fragment, or Module
    results in a web site "locator" record being created in
    the IIsWebSite table.  This means that the web site
    itself is neither installed nor uninstalled by the MSI
    package.  It does make the database available for referencing
    from a WebApplication, WebVirtualDir or WebDir record.  This allows an MSI to install
    WebApplications, WebVirtualDirs or WebDirs to already existing web sites on the machine.
    The install will fail if the web site does not exist in these cases.
  </dd>
</dl>


## Attributes
**AutoStart** (wxs:YesNoTypeUnion)
  : Specifies whether to automatically start the web site.

**ConfigureIfExists** (wxs:YesNoTypeUnion)
  : Specifies whether to configure the web site if it already exists.  Note: This will not affect uninstall behavior.  If the web site exists on uninstall, it will be removed.

**ConnectionTimeout** (xs:nonNegativeInteger)
  : Sets the timeout value for connections in seconds.

**Description** (String, required)
  : This is the name of the web site that will show up in the IIS management console.

**Directory** (String)
  : Root directory of the web site.  Resolved to a directory in the Directory table at install time by the server custom actions.

**DirProperties** (String)
  : References the Id attribute for a WebDirProperties element that specifies the security and access properties for this website root directory. This attribute may not be specified if a WebDirProperties element is directly nested in this element.

**Id** (String)
  : Identifier for the WebSite. Used within the MSI package only. If the Id is not specified, it will be generated.

**Sequence** (Integer)
  : Sequence that the web site is to be created in.

**SiteId** (String)
  : Optional attribute to directly specify the site id of the WebSite.  Use this to ensure all web sites in a web garden get the same site id.  If a number is provided, the site id must be unique on all target machines.  If "*" is used, the Description attribute will be hashed to create a unique value for the site id. This value must be a positive number or a "*" or a formatted value that resolves to "-1" (for the same behavior as "*") or a positive number or blank.  If this attribute is absent then the web site will be located using the WebAddress element associated with the web site.

**StartOnInstall** (wxs:YesNoTypeUnion)
  : Specifies whether to start the web site on install.

**WebApplication** (String)
  : Reference to a WebApplication that is to be installed as part of this web site.

**WebLog** (String)
  : Reference to WebLog definition.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)