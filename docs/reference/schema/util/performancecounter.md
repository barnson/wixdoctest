---
custom_edit_url: null
sidebar_position: 24
---
# PerformanceCounter element (Util extension)
Creates a performance counter in a performance category.

## Parents
[PerformanceCategory](performancecategory.md)

## Attributes
**Help** (String)
  : Optional help text for the performance counter.

**Language** (enumeration)
  : Language for the peformance counter name and help.  The default is to use the parent PerformanceCategory element's DefaultLanguage attribute. This attribute's value must be one of the following:
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

**Name** (String)
  : Name for the performance counter.

**Type** (enumeration)
  : Type of the performance counter. This attribute's value must be one of the following:
- *averageBase*
- *averageCount64*
- *averageTimer32*
- *counterDelta32*
- *counterTimerInverse*
- *sampleFraction*
- *timer100Ns*
- *counterTimer*
- *rawFraction*
- *timer100NsInverse*
- *counterMultiTimer*
- *counterMultiTimer100Ns*
- *counterMultiTimerInverse*
- *counterMultiTimer100NsInverse*
- *elapsedTime*
- *sampleBase*
- *rawBase*
- *counterMultiBase*
- *rateOfCountsPerSecond64*
- *rateOfCountsPerSecond32*
- *countPerTimeInterval64*
- *countPerTimeInterval32*
- *sampleCounter*
- *counterDelta64*
- *numberOfItems64*
- *numberOfItems32*
- *numberOfItemsHEX64*
- *numberOfItemsHEX32*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)