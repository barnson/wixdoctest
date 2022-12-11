---
custom_edit_url: null
sidebar_position: 6
---
# WixStandardBootstrapperApplication element (Bal extension)
Uses WixStandardBootstrapperApplication as the Bootstrapper Application for a Bundle.

## Parents
[BootstrapperApplication](../wxs/bootstrapperapplication.md)

## Attributes
**LaunchArguments** (String)
  : If set, WixStdBA will supply these arguments when launching the application specified by the LaunchTarget attribute. The string value can be formatted using Burn variables enclosed in brackets, to refer to installation directories and so forth.

**LaunchHidden** (wxs:YesNoTypeUnion)
  : If set to "yes", WixStdBA will launch the application specified by the LaunchTarget attribute with the SW_HIDE flag. This attribute is ignored when the LaunchTargetElevatedId attribute is specified.

**LaunchTarget** (String)
  : If set, the success page will show a Launch button the user can use to launch the application being installed. The string value can be formatted using Burn variables enclosed in brackets, to refer to installation directories and so forth.

**LaunchTargetElevatedId** (String)
  : Id of the target ApprovedExeForElevation element. If set with LaunchTarget, WixStdBA will launch the application through the Engine's LaunchApprovedExe method instead of through ShellExecute.

**LaunchWorkingFolder** (String)
  : WixStdBA will use this working folder when launching the specified application. The string value can be formatted using Burn variables enclosed in brackets, to refer to installation directories and so forth. This attribute is ignored when the LaunchTargetElevatedId attribute is specified.

**LicenseFile** (String)
  : Source file of the RTF license file. Cannot be used simultaneously with LicenseUrl.

**LicenseUrl** (String)
  : URL target of the license link. Cannot be used simultaneously with LicenseFile. This attribute can be empty to hide the license link completely.

**LocalizationFile** (String)
  : Source file of the theme localization .wxl file.

**LogoFile** (String)
  : Source file of the logo graphic.

**LogoSideFile** (String)
  : Source file of the side logo graphic.

**ShowVersion** (wxs:YesNoTypeUnion)
  : If set to "yes", the application version will be displayed on the UI.

**SupportCacheOnly** (wxs:YesNoTypeUnion)
  : If set to "yes", the bundle can be pre-cached using the /cache command line argument.

**SuppressDowngradeFailure** (wxs:YesNoTypeUnion)
  : If set to "yes", attempting to installer a downgraded version of a bundle will be treated as a successful do-nothing operation. The default behavior (or when explicitly set to "no") is to treat downgrade attempts as failures.

**SuppressOptionsUI** (wxs:YesNoTypeUnion)
  : If set to "yes", the Options button will not be shown and the user will not be able to choose an installation directory.

**SuppressRepair** (wxs:YesNoTypeUnion)
  : If set to "yes", the Repair button will not be shown in the maintenance-mode UI.

**Theme** (enumeration, required)
  : The built-in theme to use. This attribute's value must be one of the following:
- *hyperlinkLargeLicense*
- *hyperlinkLicense*
- *hyperlinkSidebarLicense*
- *none*
- *rtfLargeLicense*
- *rtfLicense*

**ThemeFile** (String)
  : Source file of the theme XML.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/bal.xsd)