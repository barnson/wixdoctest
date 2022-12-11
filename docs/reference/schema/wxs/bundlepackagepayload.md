---
custom_edit_url: null
sidebar_position: 29
---
# BundlePackagePayload element
Describes information about the BundlePackage payload. Cannot be specified if the owning BundlePackage specified any of SourceFile, Name, DownloadUrl, or Compressed.

## Parents
[BundlePackage](bundlepackage.md), [PayloadGroup](payloadgroup.md)

## Children
* [RemoteBundle](remotebundle.md) 

## Attributes
**CertificatePublicKey** (String)
  : Optional public key of the certificate used to sign the payload. It is not recommended to use this attribute and rely on the Hash alone.

**CertificateThumbprint** (String)
  : Optional thumbprint of the certificate used to sign the payload. It is not recommended to use this attribute and rely on the Hash alone.

**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Whether the package payload should be embedded in a container or left as an external payload.

**Description** (String)
  : Description of the file from version resources. If Hash is not specified, must not be specified.

**DownloadUrl** (String)
  : The URL to use to download the package. The following substitutions are supported:  {0} is replaced by the package Id. {1} is replaced by the payload Id. {2} is replaced by the payload file name.

**Hash** ([HexType](hextype.md 'This type supports any hexadecimal number. Both upper and lower case are supported for letters appearing in the number. This type also includes the empty string: "".'))
  : SHA-512 hash of the RemotePayload. If SourceFile is specified, must not be specified. If specified then Name, DownloadUrl, and Size are required.

**Id** (String)
  : The identifier of the package payload element.

**PayloadGeneration** (enumeration)
  : Choose one of the supported payload generation types: none, externalWithoutDownloadUrl, external, all. This attribute's value must be one of the following:
- *none*: None of the bundle's payloads or containers are automatically included as payloads for the package.
- *externalWithoutDownloadUrl*: All detached containers from the bundle that have no download url are included as payloads for the package, as well as all external payloads from the bundle that have no download url.
- *external*: All detached containers from the bundle are included as payloads for the package, as well as all external payloads from the bundle.
- *all*: All detached containers from the bundle are included as payloads for the package, as well as all other payloads that are not compressed into the detached containers. This option normally requires extra work to use since it requires all attached containers to have been extracted.

**ProductName** (String)
  : Product name of the file from version resouces. If Hash is not specified, must not be specified.

**Size** (Integer)
  : Size of the remote file in bytes. Required if Hash is specified, otherwise must not be specified.

**SourceFile** (String)
  : Location of the package to add to the bundle. The default value is the Name attribute, if provided. If Hash is specified, must not be specified.

**Version** ([VersionType](versiontype.md 'Values of this type will look like: "x.x.x.x" where x is an integer from 0 to 65534.'))
  : Version of the remote file. If Hash is not specified, must not be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)