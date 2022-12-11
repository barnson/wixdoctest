---
custom_edit_url: null
toc_max_heading_level: 2
---
# InapplicablePatchHandler Delegate
Receives an exception from «see M:WixToolset.Dtf.WindowsInstaller.Installer.DetermineApplicablePatches(System.String,System.String[],WixToolset.Dtf.WindowsInstaller.InapplicablePatchHandler,System.String,WixToolset.Dtf.WindowsInstaller.UserContexts)» indicating the reason a particular patch is not applicable to a product.
## Invoke(patch, exception) Method {#invoke_patch_exception}
Receives an exception from «see M:WixToolset.Dtf.WindowsInstaller.Installer.DetermineApplicablePatches(System.String,System.String[],WixToolset.Dtf.WindowsInstaller.InapplicablePatchHandler,System.String,WixToolset.Dtf.WindowsInstaller.UserContexts)» indicating the reason a particular patch is not applicable to a product.
### Declaration
```cs
public void Invoke(
  string patch,
  Exception exception
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| patch | string | MSP file path, XML file path, or XML blob that was passed to |
| exception | Exception | exception indicating the reason the patch is not applicable |
### Remarks
If _exception_ is an «see T:WixToolset.Dtf.WindowsInstaller.InstallerException» or subclass, then its «see P:WixToolset.Dtf.WindowsInstaller.InstallerException.ErrorCode» and «see P:WixToolset.Dtf.WindowsInstaller.InstallerException.Message» properties will indicate a more specific reason the patch was not applicable.
The _exception_ could also be a FileNotFoundException if the patch string was a file path.

### Remarks
If _exception_ is an «see T:WixToolset.Dtf.WindowsInstaller.InstallerException» or subclass, then its «see P:WixToolset.Dtf.WindowsInstaller.InstallerException.ErrorCode» and «see P:WixToolset.Dtf.WindowsInstaller.InstallerException.Message» properties will indicate a more specific reason the patch was not applicable.
The _exception_ could also be a FileNotFoundException if the patch string was a file path.

`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
