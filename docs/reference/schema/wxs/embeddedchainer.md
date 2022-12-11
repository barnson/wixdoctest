---
custom_edit_url: null
sidebar_position: 75
---
# EmbeddedChainer element


## Windows Installer references
[MsiEmbeddedChainer  Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiembeddedchainer -table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Attributes
**BinarySource** (String)
  : Reference to the Binary element that contains the chainer executable. Mutually exclusive with the FileSource and PropertySource attributes.

**CommandLine** (String)
  : Value to append to the transaction handle and passed to the chainer executable.

**FileSource** (String)
  : Reference to the File element that is the chainer executable. Mutually exclusive with the BinarySource and PropertySource attributes.

**Id** (String, required)
  : Unique identifier for embedded chainer.

**PropertySource** (String)
  : Reference to a Property that resolves to the full path to the chainer executable. Mutually exclusive with the BinarySource and FileSource attributes.


## See also
[Binary](binary.md), [File](file.md), [Property](property.md), [EmbeddedChainerRef](embeddedchainerref.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)