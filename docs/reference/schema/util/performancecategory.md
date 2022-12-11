---
custom_edit_url: null
sidebar_position: 23
---
# PerformanceCategory element (Util extension)
Used to create performance categories and configure performance counters.

## Parents
[Component](../wxs/component.md)

## Children
* [PerformanceCounter](performancecounter.md) 

## Attributes
**Close** (String)
  : Function entry point in to the Library DLL called when closing the performance counter.  The default is "ClosePerformanceData" which should be used for all managed code performance counters.

**Collect** (String)
  : Function entry point in to the Library DLL called when collecting data from the performance counter.  The default is "CollectPerformanceData" which should be used for all managed code performance counters.

**DefaultLanguage** (enumeration)
  : Default language for the performance category and contained counters' names and help text. This attribute's value must be one of the following:
- *afrikaans*
- *albanian*
- *arabic*
- *armenian*
- *assamese*
- *azeri*
- *basque*
- *belarusian*
- *bengali*
- *bulgarian*
- *catalan*
- *chinese*
- *croatian*
- *czech*
- *danish*
- *divehi*
- *dutch*
- *english*
- *estonian*
- *faeroese*
- *farsi*
- *finnish*
- *french*
- *galician*
- *georgian*
- *german*
- *greek*
- *gujarati*
- *hebrew*
- *hindi*
- *hungarian*
- *icelandic*
- *indonesian*
- *italian*
- *japanese*
- *kannada*
- *kashmiri*
- *kazak*
- *konkani*
- *korean*
- *kyrgyz*
- *latvian*
- *lithuanian*
- *macedonian*
- *malay*
- *malayalam*
- *manipuri*
- *marathi*
- *mongolian*
- *nepali*
- *norwegian*
- *oriya*
- *polish*
- *portuguese*
- *punjabi*
- *romanian*
- *russian*
- *sanskrit*
- *serbian*
- *sindhi*
- *slovak*
- *slovenian*
- *spanish*
- *swahili*
- *swedish*
- *syriac*
- *tamil*
- *tatar*
- *telugu*
- *thai*
- *turkish*
- *ukrainian*
- *urdu*
- *uzbek*
- *vietnamese*

**Help** (String)
  : Optional help text for the performance counter category.

**Id** (String)
  : Unique identifier in your installation package for this performance counter category.

**Library** (String)
  : DLL that contains the performance counter.  The default is "netfxperf.dll" which should be used for all managed code performance counters.

**MultiInstance** (wxs:YesNoTypeUnion)
  : Flag that specifies whether the performance counter category is multi or single instanced.  Default is single instance.

**Name** (String)
  : Name for the performance counter category.  If this attribute is not provided the Id attribute is used as the name of the performance counter category.

**Open** (String)
  : Function entry point in to the Library DLL called when opening the performance counter.  The default is "OpenPerformanceData" which should be used for all managed code performance counters.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)