---
custom_edit_url: null
sidebar_position: 18
---
# BootstrapperApplicationDll element
Describes the entry point to the bootstrapper application.

## Parents
[BootstrapperApplication](bootstrapperapplication.md)

## Attributes
**DpiAwareness** (enumeration)
  : The DPI awareness of the BootstrapperApplication. The default is 'perMonitorV2'. Microsoft High DPI documentation is at https://docs.microsoft.com/en-us/windows/win32/hidpi/high-dpi-desktop-application-development-on-windows. This attribute's value must be one of the following:
- *gdiScaled*: Corresponds to the .exe manifest element 'gdiScaling' with content of 'true'. Windows does not support combining this with other DPI awareness modes.
- *perMonitor*: Corresponds to the .exe manifest element 'dpiAware' with content of 'true/pm'.
- *perMonitorV2*: Corresponds to the .exe manifest element 'dpiAwareness' with content of 'PerMonitorV2, PerMonitor' and the manifest element 'dpiAware' with content of 'true/pm'.
- *system*: Corresponds to the .exe manifest element 'dpiAware' with content of 'true'.
- *unaware*

**Id** (String)
  : The identifier of BootstrapperApplicationDll element.

**Name** (String)
  : The destination path and file name for this payload. The default is the source file name. At a minimum, the Name or SourceFile attribute must be specified. This must be a relative path ('\foo' or 'C:\foo' is not allowed).

**SourceFile** (String)
  : Location of the source file. The default value is the Name attribute, if provided. At a minimum, the SourceFile or Name attribute must be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)