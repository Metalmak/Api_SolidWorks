<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ConvertStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ConvertStudy Method (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : ConvertStudy Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Name of static study to convert

*NSrcStudyType*
:   [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html).swsAnalysisStudyTypeStatic

*SNewName*
:   Name of target study to which to convert

*NTargetStudyType*
:   (see **Remarks**)

*SConfiguration*
:   Name of model configuration

*NTargetStudySubType*
:   (see **Remarks**)

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

Converts the specified static study to the specified target study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertStudy( _    ByVal SName As System.String, _    ByVal NSrcStudyType As System.Integer, _    ByVal SNewName As System.String, _    ByVal NTargetStudyType As System.Integer, _    ByVal SConfiguration As System.String, _    ByVal NTargetStudySubType As System.Integer, _    ByRef Errors As System.Integer _ ) As CWStudy ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim SName As System.String Dim NSrcStudyType As System.Integer Dim SNewName As System.String Dim NTargetStudyType As System.Integer Dim SConfiguration As System.String Dim NTargetStudySubType As System.Integer Dim Errors As System.Integer Dim value As CWStudy   value = instance.ConvertStudy(SName, NSrcStudyType, SNewName, NTargetStudyType, SConfiguration, NTargetStudySubType, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` CWStudy ConvertStudy(     System.string SName,    System.int NSrcStudyType,    System.string SNewName,    System.int NTargetStudyType,    System.string SConfiguration,    System.int NTargetStudySubType,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWStudy^ ConvertStudy(  &   System.String^ SName, &   System.int NSrcStudyType, &   System.String^ SNewName, &   System.int NTargetStudyType, &   System.String^ SConfiguration, &   System.int NTargetStudySubType, &   [Out] System.int Errors ) ``` | |

#### Parameters

*SName*
:   Name of static study to convert

*NSrcStudyType*
:   [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html).swsAnalysisStudyTypeStatic

*SNewName*
:   Name of target study to which to convert

*NTargetStudyType*
:   (see **Remarks**)

*SConfiguration*
:   Name of model configuration

*NTargetStudySubType*
:   (see **Remarks**)

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

#### Return Value

[ICWStudy](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::ConvertStudy.

# ![](dotnetimages/collapse.gif)Example

[Convert Study (VBA)](Convert_Study_Example_VB.htm)

[Convert Study (VB.NET)](Convert_Study_Example_VBNET.htm)

[Convert Study (C#)](Convert_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for SOLIDWORKS Simulation Premium.

| If NTargetStudyType is [swsAnalysisStudyType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsAnalysisStudyType_e.html)... | Then NTargetStudySubType is... |
| --- | --- |
| swsAnalysisStudyTypeDynamic | As defined in [swsDynamicAnalysisSubType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDynamicAnalysisSubType_e.html) |
| swsAnalysisStudyTypeNonlinear | * 0 = Static* 1 = Dynamic |
| swsAnalysisStudyTypeStatic | Ignored |

The following boundary conditions are transferred to the target study during conversion:

* Material properties* Connections* External loads* Fixtures* Mesh* Study properties

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudyManager::CreateNewStudy3 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~CreateNewStudy3.html)

[ICWStudyManager::DeleteStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~DeleteStudy.html)

[ICWStudyManager::DuplicateStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~DuplicateStudy.html)

[ICWStudyManager::GetStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~GetStudy.html)

[ICWStudyManager::RenameStudyFromID Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RenameStudyFromID.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0