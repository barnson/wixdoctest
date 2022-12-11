---
custom_edit_url: null
sidebar_position: 253
---
# SoftwareTag element
This extension implements the ISO/IEC 19770-2:2015 specification. A SWID tag file will be generated an inserted into the Package or Bundle.

## Parents
[Bundle](bundle.md), [Package](package.md)

## Attributes
**Bitness** ([BitnessTypeUnion](bitnesstype.md 'Values of this type will be "default", "always32" or "always64".'))
  : This attribute facilitates the installation of packages that install both 32-bit and 64-bit files. Set this attribute to 'always32' force the software id tag to a 32-bit location (such as "ProgramFilesFolder") or 'always64' to force the tag to be installed to a 64-bit location (such as "ProgramFiles64Folder").  The default value is `default` where the tag will be installed to the directory that matches the same bitness as the package.  This attribute is only allowed on a SoftwareTag element found under a Package element.

**Feature** (String)
  : Optional attribute to explicitly set the Feature when defining the software id tag in a Package. By default the software id tag will always be installed by a top-level hidden feature. It is recommended to not set this attribute.

**InstallDirectory** (String)
  : A reference to an existing Directory/@Id where the software is installed. The SWID tag file will be installed in a "swidtag" folder under that directory as per the specification. This attribute is required on a SoftwareTag element found under a Package element.

**InstallPath** (String)
  : The path where the software is installed. The SWID tag file will be installed in a "swidtag" folder. This is a formatted attribute so it is possible to use Variables as the InstallPath by setting the value to, for example, "[ProgramFilesFolder]CompanyName\Product Name". This attribute is required on a SoftwareTag element found under a Bundle element.

**Name** (String)
  : Name to use in the filename for the software id tag. By default the filename uses the Bundle/@Name or Package/@Name. If the bundle name or package name contains invalid filename characters such as ":" or "?", use this attribute to provide a valid filename.

**Regid** (String, required)
  : The regid for the software manufacturer. A regid is a URI simplified for the common case. Namely, if the scheme is "http://", it can be removed. Additionally, the domain should be minimized as much as possible (for example, remove "www." prefix if unnecessary).  For example, the WiX toolset regid is "wixtoolset.org".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)