---
custom_edit_url: null
sidebar_position: 1
---
# Certificate element (Iis extension)
Used to install and uninstall certificates.

## Parents
[Component](../wxs/component.md)

## Attributes
**BinaryRef** (String)
  : Reference to a Binary element that will store the certificate as a stream inside the package.  This attribute cannot be specified with the CertificatePath attribute.

**CertificatePath** (String)
  : If the Request attribute is "no" then this attribute is the path to the certificate file outside of the package. If the Request attribute is "yes" then this atribute is the certificate authority to request the certificate from. This attribute may be set via a formatted Property (e.g. [MyProperty]).

**Id** (String)
  : Unique identifier for this certificate in the installation package. If the Id is not specified, it will be generated.

**Name** (String, required)
  : Name of the certificate that will be installed or uninstalled in the specified store. This attribute may be set via a formatted Property (e.g. [MyProperty]).

**PFXPassword** (String)
  : If the Binary stream or path to the file outside of the package is a password protected PFX file, the password for that PFX must be specified here.  This attribute may be set via a formatted Property (e.g. [MyProperty]).

**Request** (wxs:YesNoTypeUnion)
  : This attribute controls whether the CertificatePath attribute is a path to a certificate file (Request='no') or the certificate authority to request the certificate from (Request='yes').

**StoreLocation** (enumeration, required)
  :  This attribute's value must be one of the following:
- *currentUser*
- *localMachine*

**StoreName** (enumeration, required)
  :  This attribute's value must be one of the following:
- *ca*: Contains the certificates of certificate authorities that the user trusts to issue certificates to others. Certificates in these stores are normally supplied with the operating system or by the user's network administrator.
- *my*: Use the "personal" value instead.
- *personal*: Contains personal certificates. These certificates will usually have an associated private key. This store is often referred to as the "MY" certificate store.
- *request*
- *root*: Contains the certificates of certificate authorities that the user trusts to issue certificates to others. Certificates in these stores are normally supplied with the operating system or by the user's network administrator. Certificates in this store are typically self-signed.
- *otherPeople*: Contains the certificates of those that the user normally sends enveloped messages to or receives signed messages from. See MSDN documentation for more information.
- *trustedPeople*: Contains the certificates of those directly trusted people and resources. See MSDN documentation for more information.
- *trustedPublisher*: Contains the certificates of those publishers who are trusted. See MSDN documentation for more information.

**Vital** (wxs:YesNoTypeUnion)
  : Indicates whether to fail the install if the certificate fails to install. The default is "yes".


## See also
[CertificateRef](certificateref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)