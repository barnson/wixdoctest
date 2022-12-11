---
custom_edit_url: null
sidebar_position: 1
---
# SqlDatabase element (Sql extension)
SQL Database

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Children
* [SqlFileSpec](sqlfilespec.md) 
* [SqlLogFileSpec](sqllogfilespec.md) 
* [SqlScript](sqlscript.md) 
* [SqlString](sqlstring.md) 

## Remarks
<dl>
  <dd>Nesting SqlDatabase under a Component element will result in a SqlDatabase being installed to the machine as the package is installed.</dd>
  <dd>
    Nesting SqlDatabase under Package, Fragment, or Module
    results in a database "locator" record being created in
    the SqlDatabase table.  This means that the database
    itself is neither installed nor uninstalled by the MSI
    package.  It does make the database available for referencing
    from a SqlString or SqlScript record.  This allows MSI to install
    SqlScripts or SqlStrings to already existing databases on the machine.
    The install will fail if the database does not exist in these cases.
  </dd>
  <dd>
    The User attribute references credentials specified in a User element.
    If a user is not specified then Windows Authentication will be used by default
    using the credentials of the user performing the install to execute sql
    strings, etc.
  </dd>
</dl>


## Attributes
**ConfirmOverwrite** (wxs:YesNoTypeUnion)
  : Prompt the user to overwrite the database.

**ContinueOnError** (wxs:YesNoTypeUnion)
  : Continue even if the database operation fails.

**CreateOnInstall** (wxs:YesNoTypeUnion)
  : Create the database during installation.

**CreateOnReinstall** (wxs:YesNoTypeUnion)
  : Specifies whether to create the database when the associated component is reinstalled.  Setting CreateOnInstall to yes does not imply CreateOnReinstall is set to yes.  CreateOnReinstall must be set in addition to CreateOnInstall for it to be created during both install and reinstall.

**CreateOnUninstall** (wxs:YesNoTypeUnion)
  : Create the database during uninstallation.

**Database** (String, required)
  : The name of the database. The value can be a literal value or derived from a Property element using the [Formatted](https://learn.microsoft.com/en-us/windows/win32/msi/formatted) syntax.

**DropOnInstall** (wxs:YesNoTypeUnion)
  : Drop the database during installation.

**DropOnReinstall** (wxs:YesNoTypeUnion)
  : Specifies whether to drop the database when the associated component is reinstalled.  Setting DropOnInstall to yes does not imply DropOnReinstall is set to yes.  DropOnReinstall must be set in addition to DropOnInstall for it to be dropped during both install and reinstall.

**DropOnUninstall** (wxs:YesNoTypeUnion)
  : Drop the database during uninstallation.

**Id** (String)
  : Unique identifier in your installation package for this database. If an Id is not provided, one will generated for you.

**Instance** (String)
  : Optional database server instance.

**Server** (String, required)
  : Database server name.

**User** (String)
  : Optional user used to connect to database.


## See also
[User](../util/user.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/sql.xsd)