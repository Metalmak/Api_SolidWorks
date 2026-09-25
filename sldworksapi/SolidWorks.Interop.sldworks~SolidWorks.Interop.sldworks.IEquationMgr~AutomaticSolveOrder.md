<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~AutomaticSolveOrder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutomaticSolveOrder Property (IEquationMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html) : AutomaticSolveOrder Property (IEquationMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to automatically sequence equations in an order determined by SOLIDWORKS to produce accurate results.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AutomaticSolveOrder As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEquationMgr Dim value As System.Boolean   instance.AutomaticSolveOrder = value   value = instance.AutomaticSolveOrder ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AutomaticSolveOrder {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool AutomaticSolveOrder {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to automatically sequence equations in an order determined by SOLIDWORKS to produce accurate results and to prevent changing the order in which equations are solved, false to solve equations in the order in which they appear in the equation's Ordered View and to allow changing the order in which equations are solved

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EquationMgr::AutomaticSolveOrder.

# ![](dotnetimages/collapse.gif)Example

[Automatically Solve Equations in Sequence (C#)](Automatically_Solve_Equations_in_Sequence_Example_CSharp.htm)

[Automatically Solve Equations in Sequence (VB.NET)](Automatically_Solve_Equations_in_Sequence_Example_VBNET.htm)

[Automatically Solve Equations in Sequence (VBA)](Automatically_Solve_Equations_in_Sequence_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html)

[IEquationMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr_members.html)

[IEquationMgr::Equation Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Equation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP5, Revision 20.5