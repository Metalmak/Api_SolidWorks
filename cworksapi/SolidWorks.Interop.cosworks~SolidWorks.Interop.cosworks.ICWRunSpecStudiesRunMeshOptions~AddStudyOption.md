<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions~AddStudyOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddStudyOption Method (ICWRunSpecStudiesRunMeshOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html) : AddStudyOption Method (ICWRunSpecStudiesRunMeshOptions) |

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

Adds the specified run and mesh option to the specified study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddStudyOption( _    ByVal SStudyName As System.String, _    ByVal NRunMeshOption As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRunSpecStudiesRunMeshOptions Dim SStudyName As System.String Dim NRunMeshOption As System.Integer Dim value As System.Integer   value = instance.AddStudyOption(SStudyName, NRunMeshOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddStudyOption(     System.string SStudyName,    System.int NRunMeshOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddStudyOption(  &   System.String^ SStudyName, &   System.int NRunMeshOption ) ``` | |

#### Parameters

*SStudyName*
:   Name of study

*NRunMeshOption*
:   Run and mesh option as defined in [swsRunStudiesRunMeshOptions\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptions_e.html)

#### Return Value

Error code as defined in [swsRunStudiesRunMeshOptionErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRunStudiesRunMeshOptionErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRunSpecStudiesRunMeshOptions::AddStudyOption.

# ![](dotnetimages/collapse.gif)Example

See the [ICWRunSpecStudiesRunMeshOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRunSpecStudiesRunMeshOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions.html)

[ICWRunSpecStudiesRunMeshOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRunSpecStudiesRunMeshOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0