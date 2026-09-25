<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetTotalPlies.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTotalPlies Method (ICWCompositeShellOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html) : SetTotalPlies Method (ICWCompositeShellOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NTotalPlies*
:   Total number of plies

Sets the total number of plies in the composite laminate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTotalPlies( _    ByVal NTotalPlies As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCompositeShellOptions Dim NTotalPlies As System.Integer Dim value As System.Integer   value = instance.SetTotalPlies(NTotalPlies) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetTotalPlies(     System.int NTotalPlies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetTotalPlies(  &   System.int NTotalPlies ) ``` | |

#### Parameters

*NTotalPlies*
:   Total number of plies

#### Return Value

Error code as defined in [swsCompositeShellOptionsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWCompositeShellOptions::SetTotalPlies.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWCompositeShellOptions::Sandwich](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~Sandwich.html) is set to 0.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html)

[ICWCompositeShellOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions_members.html)

[ICWCompositeShellOptions::GetTotalPlies Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetTotalPlies.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3