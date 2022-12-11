---
custom_edit_url: null
sidebar_position: 38
---
# User element (Util extension)
User for all kinds of things.  When it is not nested under a component it is included in the MSI so it can be referenced by other elements such as the User attribute in the AppPool element.  When it is nested under a Component element, the User will be created on install and can also be used for reference.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Children
* [GroupRef](groupref.md) 

## Attributes
**CanNotChangePassword** (wxs:YesNoTypeUnion)
  : The user cannot change the account's password. Equivalent to UF_PASSWD_CANT_CHANGE.

**CreateUser** (wxs:YesNoTypeUnion)
  : Indicates whether or not to create the user.  User creation can be skipped if all that is desired is to join a user to groups.

**Disabled** (wxs:YesNoTypeUnion)
  : The account is disabled. Equivalent to UF_ACCOUNTDISABLE.

**Domain** (String)
  : A [Formatted])(https://learn.microsoft.com/en-us/windows/win32/msi/formatted) string that contains the local machine or Active Directory domain for the user.

**FailIfExists** (wxs:YesNoTypeUnion)
  : Indicates if the install should fail if the user already exists.

**Id** (String)
  : 

**LogonAsBatchJob** (wxs:YesNoTypeUnion)
  : Indicates whether or not the user can logon as a batch job.  User creation can be skipped if all that is desired is to set this access right on the user.

**LogonAsService** (wxs:YesNoTypeUnion)
  : Indicates whether or not the user can logon as a serivce.  User creation can be skipped if all that is desired is to set this access right on the user.

**Name** (String, required)
  : A [Formatted])(https://learn.microsoft.com/en-us/windows/win32/msi/formatted) string that contains the name of the user account.

**Password** (String)
  : Usually a Property that is passed in on the command-line to keep it more secure.

**PasswordExpired** (wxs:YesNoTypeUnion)
  : Indicates whether the user must change their password on their first login.

**PasswordNeverExpires** (wxs:YesNoTypeUnion)
  : The account's password never expires. Equivalent to UF_DONT_EXPIRE_PASSWD.

**RemoveOnUninstall** (wxs:YesNoTypeUnion)
  : Indicates whether the user account should be removed or left behind on uninstall.

**UpdateIfExists** (wxs:YesNoTypeUnion)
  : Indicates if the user account properties should be updated if the user already exists.

**Vital** (wxs:YesNoTypeUnion)
  : Indicates whether failure to create the user or add the user to a group fails the installation. The default value is "yes".


## See also
[Group](group.md), [GroupRef](groupref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)