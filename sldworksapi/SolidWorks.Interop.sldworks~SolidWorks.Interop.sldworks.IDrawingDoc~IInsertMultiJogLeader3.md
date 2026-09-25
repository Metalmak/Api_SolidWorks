<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IInsertMultiJogLeader3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertMultiJogLeader3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : IInsertMultiJogLeader3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PointsCount*
:   Number of points

*Points*
:   Array of [points](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of size PointsCount

*StartPointArrowStyle*
:   Starting point's arrowhead style as defined in swArrowStyle\_e

*EndPointArrowStyle*
:   Ending point's arrowhead style as defined in  swArrowStyle\_e

Inserts a multi-jog leader.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertMultiJogLeader3( _    ByVal PointsCount As System.Integer, _    ByRef Points As MathPoint, _    ByVal StartPointArrowStyle As System.Integer, _    ByVal EndPointArrowStyle As System.Integer _ ) As MultiJogLeader ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim PointsCount As System.Integer Dim Points As MathPoint Dim StartPointArrowStyle As System.Integer Dim EndPointArrowStyle As System.Integer Dim value As MultiJogLeader   value = instance.IInsertMultiJogLeader3(PointsCount, Points, StartPointArrowStyle, EndPointArrowStyle) ``` | |

| C# |  |
| --- | --- |
| ``` MultiJogLeader IInsertMultiJogLeader3(     System.int PointsCount,    ref MathPoint Points,    System.int StartPointArrowStyle,    System.int EndPointArrowStyle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MultiJogLeader^ IInsertMultiJogLeader3(  &   System.int PointsCount, &   MathPoint^% Points, &   System.int StartPointArrowStyle, &   System.int EndPointArrowStyle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PointsCount*
:   Number of points

*Points*
:   Array of [points](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of size PointsCount

*StartPointArrowStyle*
:   Starting point's arrowhead style as defined in swArrowStyle\_e

*EndPointArrowStyle*
:   Ending point's arrowhead style as defined in  swArrowStyle\_e

#### Return Value

Pointer to the newly created [multi-jog leader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMultiJogLeader.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::IInsertMultiJogLeader3.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::InsertMultiJogLeader3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertMultiJogLeader3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0