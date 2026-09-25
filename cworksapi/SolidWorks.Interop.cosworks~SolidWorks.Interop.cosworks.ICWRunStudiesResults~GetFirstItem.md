<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults~GetFirstItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetFirstItem Method (ICWRunStudiesResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRunStudiesResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults.html) : GetFirstItem Method (ICWRunStudiesResults) |

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

*NRunStatus*
:   Error code of SStudyName as defined in [swsRunStudiesStatusCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesStatusCode_e.html)

Gets the first study and result code in the run studies batch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFirstItem( _    ByRef SStudyName As System.String, _    ByRef NRunStatus As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRunStudiesResults Dim SStudyName As System.String Dim NRunStatus As System.Integer Dim value As System.Integer   value = instance.GetFirstItem(SStudyName, NRunStatus) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetFirstItem(     out System.string SStudyName,    out System.int NRunStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetFirstItem(  &   [Out] System.String^ SStudyName, &   [Out] System.int NRunStatus ) ``` | |

#### Parameters

*SStudyName*
:   Name of study

*NRunStatus*
:   Error code of SStudyName as defined in [swsRunStudiesStatusCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesStatusCode_e.html)

#### Return Value

Error code as defined in [swsRunStudiesResultsErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesResultsErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRunStudiesResults::GetFirstItem.

# ![](dotnetimages/collapse.gif)Example

See the [ICWRunStudiesResults](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRunStudiesResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults.html)

[ICWRunStudiesResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults_members.html)

[ICWRunStudiesResults::GetNextItem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunStudiesResults~GetNextItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0