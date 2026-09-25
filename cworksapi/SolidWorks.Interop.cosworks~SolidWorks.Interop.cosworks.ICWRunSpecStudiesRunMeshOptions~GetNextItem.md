<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions~GetNextItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNextItem Method (ICWRunSpecStudiesRunMeshOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html) : GetNextItem Method (ICWRunSpecStudiesRunMeshOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SStudyName*
:   Name of study

*NRunMeshOption*
:   Run and mesh option as defined in [swsRunStudiesRunMeshOptions\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptions_e.html)

Gets the next item in the run studies batch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNextItem( _    ByRef SStudyName As System.String, _    ByRef NRunMeshOption As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRunSpecStudiesRunMeshOptions Dim SStudyName As System.String Dim NRunMeshOption As System.Integer Dim value As System.Integer   value = instance.GetNextItem(SStudyName, NRunMeshOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetNextItem(     out System.string SStudyName,    out System.int NRunMeshOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetNextItem(  &   [Out] System.String^ SStudyName, &   [Out] System.int NRunMeshOption ) ``` | |

#### Parameters

*SStudyName*
:   Name of study

*NRunMeshOption*
:   Run and mesh option as defined in [swsRunStudiesRunMeshOptions\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptions_e.html)

#### Return Value

Error code as defined in [swsRunStudiesRunMeshOptionErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptionErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRunSpecStudiesRunMeshOptions::GetNextItem.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html)

[ICWRunSpecStudiesRunMeshOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions_members.html)

[ICWRunSpecStudiesRunMeshOptions::GetFirstItem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions~GetFirstItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0