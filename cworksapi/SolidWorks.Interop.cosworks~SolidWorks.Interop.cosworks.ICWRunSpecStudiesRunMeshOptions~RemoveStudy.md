<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions~RemoveStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RemoveStudy Method (ICWRunSpecStudiesRunMeshOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html) : RemoveStudy Method (ICWRunSpecStudiesRunMeshOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SStudyName*
:   Name of study to remove

Removes the specified study from the run studies batch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveStudy( _    ByVal SStudyName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRunSpecStudiesRunMeshOptions Dim SStudyName As System.String Dim value As System.Integer   value = instance.RemoveStudy(SStudyName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RemoveStudy(     System.string SStudyName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RemoveStudy(  &   System.String^ SStudyName ) ``` | |

#### Parameters

*SStudyName*
:   Name of study to remove

#### Return Value

Error code as defined in [swsRunStudiesRunMeshOptionErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptionErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRunSpecStudiesRunMeshOptions::RemoveStudy.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html)

[ICWRunSpecStudiesRunMeshOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0