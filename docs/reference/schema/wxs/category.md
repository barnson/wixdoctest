---
custom_edit_url: null
sidebar_position: 30
---
# Category element
Qualified published component for parent Component

## Windows Installer references
[PublishComponent Table](https://docs.microsoft.com/en-us/windows/win32/msi/publishcomponent-table)

## Parents
[Component](component.md)

## Children
* [AppData](appdata.md) 

## Attributes
**AppData** (String)
  : An optional localizable text describing the category. The string is commonly parsed by the application and can be displayed to the user. It should describe the category.

**Feature** (String)
  : Feature that controls the advertisement of the category. Defaults to the primary Feature for the parent Component .

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : A string GUID that represents the category of components being grouped together.

**Qualifier** (String, required)
  : A text string that qualifies the value in the Id attribute. A qualifier is used to distinguish multiple forms of the same Component, such as a Component that is implemented in multiple languages.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)