<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~GetResultFolderPath2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetResultFolderPath2 Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : GetResultFolderPath2 Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SResultFolderPath*
:   Path to the results folder

Gets the path to the folder that stores the results of this dynamic study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetResultFolderPath2( _    ByRef SResultFolderPath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim SResultFolderPath As System.String Dim value As System.Integer   value = instance.GetResultFolderPath2(SResultFolderPath) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetResultFolderPath2(     out System.string SResultFolderPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetResultFolderPath2(  &   [Out] System.String^ SResultFolderPath ) ``` | |

#### Parameters

*SResultFolderPath*
:   Path to the results folder

#### Return Value

0 indicates success; a non-0 value indicates failure

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::GetResultFolderPath2.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

[ICWDynamicStudyOptions::SetResultFolderPath2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetResultFolderPath2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0