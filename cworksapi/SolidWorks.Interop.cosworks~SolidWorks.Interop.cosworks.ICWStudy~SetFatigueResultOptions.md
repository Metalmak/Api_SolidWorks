<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~SetFatigueResultOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFatigueResultOptions Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : SetFatigueResultOptions Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFatigueCalculationsOption*
:   Fatigue calculation option as defined in [swsFatigueCalculationsOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueCalculationsOption_e.html)

*DispArray*
:   Array of vertices and reference points at which to plot damage matrix charts; only valid in variable amplitude fatigue studies

Sets the result options for this fatigue study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFatigueResultOptions( _    ByVal NFatigueCalculationsOption As System.Integer, _    ByVal DispArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim NFatigueCalculationsOption As System.Integer Dim DispArray As System.Object Dim value As System.Integer   value = instance.SetFatigueResultOptions(NFatigueCalculationsOption, DispArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFatigueResultOptions(     System.int NFatigueCalculationsOption,    System.object DispArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFatigueResultOptions(  &   System.int NFatigueCalculationsOption, &   System.Object^ DispArray ) ``` | |

#### Parameters

*NFatigueCalculationsOption*
:   Fatigue calculation option as defined in [swsFatigueCalculationsOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueCalculationsOption_e.html)

*DispArray*
:   Array of vertices and reference points at which to plot damage matrix charts; only valid in variable amplitude fatigue studies

#### Return Value

0 if successful, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::SetFatigueResultOptions.

# ![](dotnetimages/collapse.gif)Example

[Create Fatigue Study (VBA)](Create_Fatigue_Study_Example_VB.htm)

[Create Fatigue Study (VB.NET)](Create_Fatigue_Study_Example_VBNET.htm)

[Create Fatigue Study (C#)](Create_Fatigue_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::FatigueStudyOptions Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~FatigueStudyOptions.html)

[ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html)

[ICWFatigueStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueStudyOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0