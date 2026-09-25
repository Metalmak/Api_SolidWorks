<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~DuplicateStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DuplicateStudy Method (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : DuplicateStudy Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Name of study to duplicate

*SNewName*
:   Name of new study

*SConfiguration*
:   Name of configuration

*NNLDynamic*
:   1 to copy to a nonlinear dynamic study, 0 to not

*Errors*
:   Error code as defined in [swsDuplicateStudyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDuplicateStudyError_e.html)

Duplicates the specified study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DuplicateStudy( _    ByVal SName As System.String, _    ByVal SNewName As System.String, _    ByVal SConfiguration As System.String, _    ByVal NNLDynamic As System.Integer, _    ByRef Errors As System.Integer _ ) As CWStudy ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim SName As System.String Dim SNewName As System.String Dim SConfiguration As System.String Dim NNLDynamic As System.Integer Dim Errors As System.Integer Dim value As CWStudy   value = instance.DuplicateStudy(SName, SNewName, SConfiguration, NNLDynamic, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` CWStudy DuplicateStudy(     System.string SName,    System.string SNewName,    System.string SConfiguration,    System.int NNLDynamic,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWStudy^ DuplicateStudy(  &   System.String^ SName, &   System.String^ SNewName, &   System.String^ SConfiguration, &   System.int NNLDynamic, &   [Out] System.int Errors ) ``` | |

#### Parameters

*SName*
:   Name of study to duplicate

*SNewName*
:   Name of new study

*SConfiguration*
:   Name of configuration

*NNLDynamic*
:   1 to copy to a nonlinear dynamic study, 0 to not

*Errors*
:   Error code as defined in [swsDuplicateStudyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDuplicateStudyError_e.html)

#### Return Value

[ICWStudy](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::DuplicateStudy.

# ![](dotnetimages/collapse.gif)Example

[Duplicate Study (VBA)](Duplicate_Study_Example_VB.htm)

[Duplicate Study (VB.NET)](Duplicate_Study_Example_VBNET.htm)

[Duplicate Study (C#)](Duplicate_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

[ICWStudyManager::GetStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~GetStudy.html)

[ICWStudyManager::CreateNewStudy3 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~CreateNewStudy3.html)

[ICWStudyManager::DeleteStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~DeleteStudy.html)

[ICWStudyManager::RenameStudyFromID Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~RenameStudyFromID.html)

[ICWStudyManager::ConvertStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~ConvertStudy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0