<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~SetAutomaticSolve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAutomaticSolve Method (ISketch) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : SetAutomaticSolve Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SolveFlag*
:   True if solving is on, false if it is off

Controls whether the computation to solve the sketch geometry of the part as modifications are automatically performed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAutomaticSolve( _    ByVal SolveFlag As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim SolveFlag As System.Boolean Dim value As System.Boolean   value = instance.SetAutomaticSolve(SolveFlag) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetAutomaticSolve(     System.bool SolveFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetAutomaticSolve(  &   System.bool SolveFlag ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SolveFlag*
:   True if solving is on, false if it is off

#### Return Value

True if set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::SetAutomaticSolve.

# ![](dotnetimages/collapse.gif)Remarks

If an application is making many changes in a sketch, then the Automatic Solve option may be turned off temporarily. After changes are completed, this option should be restored to its previous value, which can be obtained by calling [ISketch::GetAutomaticSolve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~GetAutomaticSolve.html) before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)

[IModelDoc2::AutoSolveToggle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AutoSolveToggle.html)