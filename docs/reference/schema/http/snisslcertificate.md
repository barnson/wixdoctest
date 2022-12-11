---
custom_edit_url: null
sidebar_position: 1
---
# SniSslCertificate element (Http extension)
Associates an SNI SSL certificate with HTTP.SYS.

## Parents
[Component](../wxs/component.md)

## Attributes
**AppId** (String)
  : A GUID used ot identify the SNI SSL binding.

**HandleExisting** (enumeration)
  : Rights for this ACE. Default is "all". This attribute's value must be one of the following:
- *replace*
- *ignore*
- *fail*

**Host** (String, required)
  : Host of the URL to bind with the SNI SSL certificate.

**Id** (String)
  : Unique ID of this SNI SSL. If this attribute is not specified, an identifier will be generated automatically.

**Port** (String, required)
  : Host of the URL to bind with the SNI SSL certificate.

**Store** (String)
  : Certificate store containing the SNI SSL certificate.

**Thumbprint** (String, required)
  : Thumbprint of the SNI SSL certificate.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/http.xsd)