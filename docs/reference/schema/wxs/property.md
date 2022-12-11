---
custom_edit_url: null
sidebar_position: 183
---
# Property element
Property value for a Package or Module.

## Windows Installer references
[Property Table](https://docs.microsoft.com/en-us/windows/win32/msi/property-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [ODBCDataSource](odbcdatasource.md), [ODBCDriver](odbcdriver.md), [Upgrade](upgrade.md), [Control](control.md), [UI](ui.md)

## Children
* [ComplianceDrive](compliancedrive.md) (no more than 1) : Starts searches from the CCP_DRIVE.
* [ComponentSearch](componentsearch.md) 
* [DirectorySearch](directorysearch.md) 
* [DirectorySearchRef](directorysearchref.md) 
* [IniFileSearch](inifilesearch.md) 
* [ProductSearch](productsearch.md) 
* [RegistrySearch](registrysearch.md) 
* [RegistrySearchRef](registrysearchref.md) 

## Attributes
**Admin** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Denotes that the Property is saved during admininistrative installation. See the AdminProperties Property for more information.

**ComplianceCheck** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Adds a row to the CCPSearch table. This attribute is only valid when this Property contains a search element.

**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Denotes that the Property is not logged during installation. See the MsiHiddenProperties Property for more information.

**Id** (String, required)
  : Unique identifier for Property.

**Secure** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Denotes that the Property can be passed to the server side when doing a managed installation with elevated privileges. See the SecureCustomProperties Property for more information.

**SuppressModularization** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use to suppress modularization of this property identifier in merge modules. Using this functionality is strongly discouraged; it should only be necessary as a workaround of last resort in rare scenarios.

**Value** (String)
  : Sets a default value for the property. The value will be overwritten if the Property is used for a search.


## See also
[PropertyRef](propertyref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)