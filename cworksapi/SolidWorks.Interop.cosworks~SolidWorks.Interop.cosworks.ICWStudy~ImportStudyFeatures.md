<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ImportStudyFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ImportStudyFeatures Method (ICWStudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : ImportStudyFeatures Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SComponent*
:   Name of the assembly component from whose study to import study features

*SStudy*
:   Name of SComponent's study from which to import study features

*SConfig*
:   Name of SComponent's configuration

*NFilter*
:   Study features to import as defined in [swsImportStudyFeaturesFilterType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsImportStudyFeaturesErrorCode_e.html)

*BPropagate*
:   True to propagate imported study features to components in this study that are similar to SComponent, false to not

*ErrorCode*
:   Result code as defined in [swsImportStudyFeaturesErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsImportStudyFeaturesErrorCode_e.html)

Imports the study features of the specified component's study into this study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportStudyFeatures( _    ByVal SComponent As System.String, _    ByVal SStudy As System.String, _    ByVal SConfig As System.String, _    ByVal NFilter As System.Integer, _    ByVal BPropagate As System.Boolean, _    ByRef ErrorCode As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim SComponent As System.String Dim SStudy As System.String Dim SConfig As System.String Dim NFilter As System.Integer Dim BPropagate As System.Boolean Dim ErrorCode As System.Integer Dim value As System.Boolean   value = instance.ImportStudyFeatures(SComponent, SStudy, SConfig, NFilter, BPropagate, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImportStudyFeatures(     System.string SComponent,    System.string SStudy,    System.string SConfig,    System.int NFilter,    System.bool BPropagate,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ImportStudyFeatures(  &   System.String^ SComponent, &   System.String^ SStudy, &   System.String^ SConfig, &   System.int NFilter, &   System.bool BPropagate, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SComponent*
:   Name of the assembly component from whose study to import study features

*SStudy*
:   Name of SComponent's study from which to import study features

*SConfig*
:   Name of SComponent's configuration

*NFilter*
:   Study features to import as defined in [swsImportStudyFeaturesFilterType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsImportStudyFeaturesErrorCode_e.html)

*BPropagate*
:   True to propagate imported study features to components in this study that are similar to SComponent, false to not

*ErrorCode*
:   Result code as defined in [swsImportStudyFeaturesErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsImportStudyFeaturesErrorCode_e.html)

#### Return Value

VARIANT\_TRUE (-1) if successful, VARIANT\_FALSE (0) if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::ImportStudyFeatures.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2018 SP0