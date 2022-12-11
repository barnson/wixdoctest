---
custom_edit_url: null
sidebar_position: 174
---
# Payload element
Describes a payload to a bootstrapper.

## Parents
[BootstrapperApplication](bootstrapperapplication.md), [BootstrapperApplicationRef](bootstrapperapplicationref.md), [BundleExtension](bundleextension.md), [MsiPackage](msipackage.md), [MspPackage](msppackage.md), [MsuPackage](msupackage.md), [ExePackage](exepackage.md), [BundlePackage](bundlepackage.md), [PayloadGroup](payloadgroup.md)

## Attributes
**CertificatePublicKey** (String)
  : Optional public key of the certificate used to sign the payload. It is not recommended to use this attribute and rely on the Hash alone.

**CertificateThumbprint** (String)
  : Optional thumbprint of the certificate used to sign the payload. It is not recommended to use this attribute and rely on the Hash alone.

**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Whether the payload should be embedded in a container or left as an external payload.

**DownloadUrl** (String)
  : The URL to use to download the package. The following substitutions are supported:  {0} is replaced by the package Id. {1} is replaced by the payload Id. {2} is replaced by the payload file name.

**Hash** (String)
  : Optional SHA256 hash of the payload. Must be provided if the SourceFile attribute is not used.

**Id** (String)
  : The identifier of Payload element.

**Name** (String)
  : The destination path and file name for this payload. The default is the source file name. At a minimum, the Name or SourceFile attribute must be specified. This must be a relative path ('\foo' or 'C:\foo' is not allowed).

**SourceFile** (String)
  : Location of the source file. The default value is the Name attribute, if provided. At a minimum, the SourceFile or Name attribute must be specified.

**BAFunctions** (wxs:YesNoTypeUnion)
  : When set to "yes", WixStdBA will load the DLL and work with it to handle BA messages. Only one payload may be marked with this attribute set to "yes".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)