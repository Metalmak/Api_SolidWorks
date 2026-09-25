<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~CreateNewStudy3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateNewStudy3 Method (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : CreateNewStudy3 Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   New study name

*NAnalysisType*
:   Type of study as defined in [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html)

*NStudySubOptions*
:   | If NAnalysisType is ... | Then NStudySubOptions is a sub-study as defined in ... |
    | --- | --- |
    | swsAnalysisStudyType\_e.swsAnalysisStudyTypeDynamic | [swsDynamicAnalysisSubType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDynamicAnalysisSubType_e.html) |
    | swsAnalysisStudyType\_e.swsAnalysisStudyTypeFatigue | [swsFatigueStudySubOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueStudySubOption_e.html) |

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

Creates a new study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateNewStudy3( _    ByVal SName As System.String, _    ByVal NAnalysisType As System.Integer, _    ByVal NStudySubOptions As System.Integer, _    ByRef Errors As System.Integer _ ) As CWStudy ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim SName As System.String Dim NAnalysisType As System.Integer Dim NStudySubOptions As System.Integer Dim Errors As System.Integer Dim value As CWStudy   value = instance.CreateNewStudy3(SName, NAnalysisType, NStudySubOptions, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` CWStudy CreateNewStudy3(     System.string SName,    System.int NAnalysisType,    System.int NStudySubOptions,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWStudy^ CreateNewStudy3(  &   System.String^ SName, &   System.int NAnalysisType, &   System.int NStudySubOptions, &   [Out] System.int Errors ) ``` | |

#### Parameters

*SName*
:   New study name

*NAnalysisType*
:   Type of study as defined in [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html)

*NStudySubOptions*
:   | If NAnalysisType is ... | Then NStudySubOptions is a sub-study as defined in ... |
    | --- | --- |
    | swsAnalysisStudyType\_e.swsAnalysisStudyTypeDynamic | [swsDynamicAnalysisSubType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDynamicAnalysisSubType_e.html) |
    | swsAnalysisStudyType\_e.swsAnalysisStudyTypeFatigue | [swsFatigueStudySubOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueStudySubOption_e.html) |

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

#### Return Value

[ICWStudy](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudy.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::CreateNewStudy3.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

[Create Fatigue Study (VBA)](Create_Fatigue_Study_Example_VB.htm)

[Create Fatigue Study (VB.NET)](Create_Fatigue_Study_Example_VBNET.htm)

[Create Fatigue Study (C#)](Create_Fatigue_Study_Example_CSharp.htm)

[Add Remote Load (VBA)](Add_Remote_Load_Example_VB.htm)

[Add Remote Load (VB.NET)](Add_Remote_Load_Example_VBNET.htm)

[Add Remote Load (C#)](Add_Remote_Load_Example_CSharp.htm)

[Create Drop Test Study (VBA)](Create_Drop_Test_Study_Example_VB.htm)

[Create Drop Test Study (VB.NET)](Create_Drop_Test_Study_Example_VBNET.htm)

[Create Drop Test Study (C#)](Create_Drop_Test_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudyManager::DuplicateStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~DuplicateStudy.html)

[ICWStudyManager::ConvertStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ConvertStudy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0