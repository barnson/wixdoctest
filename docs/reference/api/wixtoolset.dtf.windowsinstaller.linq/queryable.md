---
custom_edit_url: null
toc_max_heading_level: 2
---
# Queryable Class
Allows any Database instance to be converted into a queryable database.
## Methods
| Method | Description |
| ------ | ----------- |
| [AsQueryable(db)](#asqueryable_db) | Converts any Database instance into a queryable database. |
`WixToolset.Dtf.WindowsInstaller.Linq.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## AsQueryable(db) Method {#asqueryable_db}
Converts any Database instance into a queryable database.
### Declaration
```cs
public static QDatabase AsQueryable(
  WixToolset.Dtf.WindowsInstaller.Database db
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| db | WixToolset.Dtf.WindowsInstaller.Database |  |
### Return value
`QDatabase` Queryable database instance that operates on the same MSI handle.
### Remarks
This extension method is meant for convenient on-the-fly conversion. If the existing database instance already happens to be a QDatabase, then it is returned unchanged. Otherwise since the new database carries the same MSI handle, only one of the instances needs to be closed, not both.
