<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetRelatedTangentEdges.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetRelatedTangentEdges Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetRelatedTangentEdges Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BendLine*
:   Bendline whose visible tangent edges you want (see **Remarks**)

*NumOfTangentEdges*
:   Number of visible tangent edges for the specified bendline

Gets the visible tangent edges for the specified bendline in a [flat-pattern drawing view](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IsFlatPatternView.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetRelatedTangentEdges( _    ByVal BendLine As SketchSegment, _    ByVal NumOfTangentEdges As System.Integer _ ) As Edge ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim BendLine As SketchSegment Dim NumOfTangentEdges As System.Integer Dim value As Edge   value = instance.IGetRelatedTangentEdges(BendLine, NumOfTangentEdges) ``` | |

| C# |  |
| --- | --- |
| ``` Edge IGetRelatedTangentEdges(     SketchSegment BendLine,    System.int NumOfTangentEdges ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Edge^ IGetRelatedTangentEdges(  &   SketchSegment^ BendLine, &   System.int NumOfTangentEdges ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BendLine*
:   Bendline whose visible tangent edges you want (see **Remarks**)

*NumOfTangentEdges*
:   Number of visible tangent edges for the specified bendline

#### Return Value

* in-process, unmanaged C++: Pointer to an array of visible tangent [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) for the specified bendline* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IView::GetRelatedTangentEdgeCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetRelatedTangentEdgeCount.html) to get NumOfTangentEdges.

Hidden tangent edges are not returned by this method. Call [IDrawingDoc::ViewTangentEdges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~ViewTangentEdges.html) to change the visibility of tangent edges in a drawing.

Call [IView::GetBendLineCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetBendLineCount.html) to get the number of bendlines in a flat-pattern drawing view. Call [IView::GetBendLines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetBendLines.html) or [IView::IGetBendLines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetBendLines.html) to get an array of bendlines for a flat-pattern drawing view. Use the value returned by IView::GetBendLineCount to determine the index of the bendline in the array of bendlines you want.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetRelatedTangentEdges Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetRelatedTangentEdges.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0