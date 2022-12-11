---
custom_edit_url: null
sidebar_position: 3
---
# UrlReservation element (Http extension)
Makes a reservation record for the HTTP Server API configuration store on Windows XP SP2, Windows Server 2003, and later.  For more information about the HTTP Server API, see [HTTP Server API](https://learn.microsoft.com/en-us/windows/win32/http/http-api-start-page).

## Parents
[Component](../wxs/component.md), [ServiceInstall](../wxs/serviceinstall.md)

## Children
* [UrlAce](urlace.md) 

## Attributes
**HandleExisting** (enumeration)
  : Specifies the behavior when trying to install a URL reservation and it already exists. This attribute's value must be one of the following:
- *replace*: Replaces the existing URL reservation (the default).
- *ignore*: Keeps the existing URL reservation.
- *fail*: The installation fails.

**Id** (String)
  : Unique ID of this URL reservation. If this attribute is not specified, an identifier will be generated automatically.

**Sddl** (String)
  : Security descriptor to apply to the URL reservation. Can't be specified when using children UrlAce elements.

**Url** (String, required)
  : The [UrlPrefix](https://learn.microsoft.com/en-us/windows/win32/http/urlprefix-strings) string that defines the portion of the URL namespace to which this reservation pertains.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/http.xsd)