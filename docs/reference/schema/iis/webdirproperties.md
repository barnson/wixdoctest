---
custom_edit_url: null
sidebar_position: 11
---
# WebDirProperties element (Iis extension)
WebDirProperties used by one or more WebSites. Lists properties common to IIS web sites and vroots. Corresponding properties can be viewed through the IIS Manager snap-in. One property entry can be reused by multiple sites or vroots using the Id field as a reference, using WebVirtualDir.DirProperties, WebSite.DirProperties, or WebDir.DirProperties.

## Parents
[Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md), [WebVirtualDir](webvirtualdir.md), [WebDir](webdir.md), [WebSite](website.md)

## Attributes
**AccessSSL** (wxs:YesNoTypeUnion)
  : A value of true indicates that file access requires SSL file permission processing, with or without a client certificate. This corresponds to AccessSSL flag for AccessSSLFlags IIS metabase property.

**AccessSSL128** (wxs:YesNoTypeUnion)
  : A value of true indicates that file access requires SSL file permission processing with a minimum key size of 128 bits, with or without a client certificate. This corresponds to AccessSSL128 flag for AccessSSLFlags IIS metabase property.

**AccessSSLMapCert** (wxs:YesNoTypeUnion)
  : This corresponds to AccessSSLMapCert flag for AccessSSLFlags IIS metabase property.

**AccessSSLNegotiateCert** (wxs:YesNoTypeUnion)
  : This corresponds to AccessSSLNegotiateCert flag for AccessSSLFlags IIS metabase property.

**AccessSSLRequireCert** (wxs:YesNoTypeUnion)
  : This corresponds to AccessSSLRequireCert flag for AccessSSLFlags IIS metabase property.

**AnonymousAccess** (wxs:YesNoTypeUnion)
  : Sets the Enable Anonymous Access checkbox, which maps anonymous users to a Windows user account. When setting this to 'yes' you should also provide the user account using the AnonymousUser attribute, and determine what setting to use for the IIsControlledPassword attribute. Defaults to 'no.'

**AnonymousUser** (String)
  : Reference to the Id attribute on the User element to be used as the anonymous user for the directory. See the User element for more information.

**AspDetailedError** (wxs:YesNoTypeUnion)
  : Sets the option for whether to send detailed ASP errors back to the client on script error. Default is 'no.'

**AuthenticationProviders** (String)
  : Comma delimited list, in order of precedence, of Windows authentication providers that IIS will attempt to use: NTLM, Kerberos, Negotiate, and others.

**BasicAuthentication** (wxs:YesNoTypeUnion)
  : Sets the Basic Authentication option, which allows clients to provide credentials in plaintext over the wire. Defaults to 'no.'

**CacheControlCustom** (String)
  : Custom HTTP 1.1 cache control directives.

**CacheControlMaxAge** (xs:nonNegativeInteger)
  : Integer value specifying the cache control maximum age value.

**ClearCustomError** (wxs:YesNoTypeUnion)
  : Specifies whether IIs will return custom errors for this directory.

**DefaultDocuments** (String)
  : The list of default documents to set for this web directory, in comma-delimited format.

**DigestAuthentication** (wxs:YesNoTypeUnion)
  : Sets the Digest Authentication option, which allows using digest authentication with domain user accounts. Defaults to 'no.'

**Execute** (wxs:YesNoTypeUnion)
  : 

**HttpExpires** (String)
  : Value to set the HttpExpires attribute to for a Web Dir in the metabase.

**Id** (String)
  : Identifier for the WebDirProperties. The Id is required when the parent is a Fragment, Module, or Package. Otherwise, Id is optional and if not specified, it will be generated.

**IIsControlledPassword** (wxs:YesNoTypeUnion)
  : Sets whether IIS should control the password used for the Windows account specified in the AnonymousUser attribute. Defaults to 'no.'

**Index** (wxs:YesNoTypeUnion)
  : Sets the Index Resource option, which specifies whether this web directory should be indexed. Defaults to 'no.'

**LogVisits** (wxs:YesNoTypeUnion)
  : Sets whether visits to this site should be logged. Defaults to 'no.'

**PassportAuthentication** (wxs:YesNoTypeUnion)
  : Sets the Passport Authentication option, which allows clients to provide credentials via a .Net Passport account. Defaults to 'no.'

**Read** (wxs:YesNoTypeUnion)
  : 

**Script** (wxs:YesNoTypeUnion)
  : 

**WindowsAuthentication** (wxs:YesNoTypeUnion)
  : Sets the Windows Authentication option, which enables integrated Windows authentication to be used on the site. Defaults to 'no.'

**Write** (wxs:YesNoTypeUnion)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)