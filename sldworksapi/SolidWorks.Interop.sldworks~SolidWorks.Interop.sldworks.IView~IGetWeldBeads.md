<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetWeldBeads.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetWeldBeads Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetWeldBeads Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumWeldBead*
:   Total number of weld beads on this drawing view

Gets all of the weld beads on this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetWeldBeads( _    ByVal NumWeldBead As System.Integer _ ) As WeldBead ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim NumWeldBead As System.Integer Dim value As WeldBead   value = instance.IGetWeldBeads(NumWeldBead) ``` | |

| C# |  |
| --- | --- |
| ``` WeldBead IGetWeldBeads(     System.int NumWeldBead ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` WeldBead^ IGetWeldBeads(  &   System.int NumWeldBead ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumWeldBead*
:   Total number of weld beads on this drawing view

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [weld beads](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldBead.html)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Use this method to obtain the array of weld beads all at once instead of calling [IView::GetFirstWeldBead](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFirstWeldBead.html) and then repeatedly calling [IWeldBead::GetNext](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldBead~GetNext.html) to obtain the weld beads in the drawing view.

Before calling this method, call [IView::GetWeldBeadCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetWeldBeadCount.html) to get the value for numWeldBead.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetWeldBeads Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetWeldBeads.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP1, Revision Number 17.1