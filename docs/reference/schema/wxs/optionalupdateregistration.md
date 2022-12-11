---
custom_edit_url: null
sidebar_position: 156
---
# OptionalUpdateRegistration element
Writes additional information to the Windows registry that can be used to detect the bundle. This registration is intended primarily for update to an existing product.

## Parents
[Bundle](bundle.md)

## Remarks
<p>The attributes are used to write the following registry values to the key:
<code>SOFTWARE\[Manufacturer]\Updates\[ProductFamily]\[Name]</code></p>
<ul>
  <li>ThisVersionInstalled: Y</li>
  <li>PackageName: &gt;bundle name&lt;</li>
  <li>PackageVersion: &gt;bundle version&lt;</li>
  <li>Publisher: [Manufacturer]</li>
  <li>PublishingGroup: [Department]</li>
  <li>ReleaseType: [Classification]</li>
  <li>InstalledBy: [LogonUser]</li>
  <li>InstalledDate: [Date]</li>
  <li>InstallerName: &gt;installer name&lt;</li>
  <li>InstallerVersion: &gt;installer version&lt;</li>
</ul>


## Attributes
**Classification** (String)
  : The release type of the update bundle, such as Update, Security Update, Service Pack, etc. The default value is Update.

**Department** (String)
  : The name of the department or division publishing the update bundle. The PublishingGroup registry value is not written if this attribute is not specified.

**Manufacturer** (String)
  : The name of the manufacturer. The default is the Bundle/@Manufacturer attribute, but may also be a short form, ex: Acme instead of Acme Corporation. An error is generated at build time if neither attribute is specified.

**Name** (String)
  : The name of the bundle. The default is the Bundle/@Name attribute, but may also be a short form, ex: KB12345 instead of Update to Product (KB12345). An error is generated at build time if neither attribute is specified.

**ProductFamily** (String)
  : The name of the family of products being updated. The default is the Bundle/@ParentName attribute. The corresponding registry key is not created if neither attribute is specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)