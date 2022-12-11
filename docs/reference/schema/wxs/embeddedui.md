---
custom_edit_url: null
sidebar_position: 77
---
# EmbeddedUI element
Element value is the condition. Use CDATA if message contains delimiter characters.

## Windows Installer references
[MsiEmbeddedUI Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiembeddedui-table)

## Parents
[UI](ui.md)

## Children
* [EmbeddedUIResource](embeddeduiresource.md) 

## Attributes
**Id** (String)
  : Unique identifier for embedded UI.If this attribute is not specified the Name attribute or the file name portion of the SourceFile attribute will be used.

**IgnoreActionData** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_ACTIONDATA messages.

**IgnoreActionStart** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_ACTIONSTART messages.

**IgnoreCommonData** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_COMMONDATA messages.

**IgnoreError** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_ERROR messages.

**IgnoreFatalExit** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_FATALEXIT messages.

**IgnoreFilesInUse** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_FILESINUSE messages.

**IgnoreInfo** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_INFO messages.

**IgnoreInitialize** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_INITIALIZE messages.

**IgnoreInstallEnd** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_INSTALLEND messages.

**IgnoreInstallStart** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_INSTALLSTART messages.

**IgnoreOutOfDiskSpace** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_OUTOFDISKSPACE messages.

**IgnoreProgress** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_PROGRESS messages.

**IgnoreResolveSource** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_RESOLVESOURCE messages.

**IgnoreRMFilesInUse** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_RMFILESINUSE messages.

**IgnoreShowDialog** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_SHOWDIALOG messages.

**IgnoreTerminate** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_TERMINATE messages.

**IgnoreUser** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_USER messages.

**IgnoreWarning** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Embedded UI will not recieve any INSTALLLOGMODE_WARNING messages.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The name for the embedded UI DLL when it is extracted from the MSI package and executed. (Windows Installer does not support the typical short filename and long filename combination for embedded UI files as it does for other kinds of files.) If this attribute is not specified the file name portion of the SourceFile attribute will be used.

**SourceFile** (String, required)
  : Path to the binary file that is the embedded UI. This must be a DLL that exports the following three entry points: InitializeEmbeddedUI, EmbeddedUIHandler and ShutdownEmbeddedUI.

**SupportBasicUI** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set yes to allow the Windows Installer to display the embedded UI during basic UI level installation.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)