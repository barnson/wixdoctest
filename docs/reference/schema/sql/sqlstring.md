---
custom_edit_url: null
sidebar_position: 5
---
# SqlString element (Sql extension)
SQL String

## Parents
[Component](../wxs/component.md), [SqlDatabase](sqldatabase.md)

## Attributes
**ContinueOnError** (wxs:YesNoTypeUnion)
  : Continue executing strings even if this one fails.

**ExecuteOnInstall** (wxs:YesNoTypeUnion)
  : Specifies to execute the string when the associated component is installed.  This attribute is mutually exclusive with the RollbackOnInstall, RollbackOnReinstall and RollbackOnUninstall attributes.

**ExecuteOnReinstall** (wxs:YesNoTypeUnion)
  : Specifies whether to execute the string when the associated component is reinstalled.  Setting ExecuteOnInstall to yes does not imply ExecuteOnReinstall is set to yes.  ExecuteOnReinstall must be set in addition to ExecuteOnInstall for it to be executed during both install and reinstall.  This attribute is mutually exclusive with the RollbackOnInstall, RollbackOnReinstall and RollbackOnUninstall attributes.

**ExecuteOnUninstall** (wxs:YesNoTypeUnion)
  : Specifies to execute the string when the associated component is uninstalled.  This attribute is mutually exclusive with the RollbackOnInstall, RollbackOnReinstall and RollbackOnUninstall attributes.

**Id** (String)
  : Unique identifier in your installation package for this sql command. If an Id is not provided, one will generated for you.

**RollbackOnInstall** (wxs:YesNoTypeUnion)
  : Specifies whether to execute the string on rollback if an attempt is made to install the associated component.  This attribute is mutually exclusive with the ExecuteOnInstall, ExecuteOnReinstall and ExecuteOnUninstall attributes.

**RollbackOnReinstall** (wxs:YesNoTypeUnion)
  : Specifies whether to execute the string on rollback if an attempt is made to reinstall the associated component.  This attribute is mutually exclusive with the ExecuteOnInstall, ExecuteOnReinstall and ExecuteOnUninstall attributes.

**RollbackOnUninstall** (wxs:YesNoTypeUnion)
  : Specifies whether to execute the string on rollback if an attempt is made to uninstall the associated component.  This attribute is mutually exclusive with the ExecuteOnInstall, ExecuteOnReinstall and ExecuteOnUninstall attributes.

**Sequence** (Integer)
  : Specifes the order to run the SQL Strings.  It is recommended that rollback strings be scheduled before their complementary execution string.  This order is also relative across the SqlScript element.

**SQL** (String, required)
  : SQL command to execute against the database.

**SqlDb** (String)
  : Id of the SqlDatabase to execute the script against. Required when not child of SqlDatabase.

**User** (String)
  : Optional user used to connect to database.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/sql.xsd)