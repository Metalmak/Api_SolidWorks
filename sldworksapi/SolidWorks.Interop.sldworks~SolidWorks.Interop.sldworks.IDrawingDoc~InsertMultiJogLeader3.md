<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertMultiJogLeader3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMultiJogLeader3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertMultiJogLeader3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Points*
:   Array of [points](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of size PointsCount

*StartPointArrowStyle*
:   Starting point's arrowhead style as defined in swArrowStyle\_e

*EndPointArrowStyle*
:   Ending point's arrowhead style as defined in  swArrowStyle\_e

Inserts a multi-jog leader.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMultiJogLeader3( _    ByVal Points As System.Object, _    ByVal StartPointArrowStyle As System.Integer, _    ByVal EndPointArrowStyle As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Points As System.Object Dim StartPointArrowStyle As System.Integer Dim EndPointArrowStyle As System.Integer Dim value As System.Object   value = instance.InsertMultiJogLeader3(Points, StartPointArrowStyle, EndPointArrowStyle) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertMultiJogLeader3(     System.object Points,    System.int StartPointArrowStyle,    System.int EndPointArrowStyle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertMultiJogLeader3(  &   System.Object^ Points, &   System.int StartPointArrowStyle, &   System.int EndPointArrowStyle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Points*
:   Array of [points](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of size PointsCount

*StartPointArrowStyle*
:   Starting point's arrowhead style as defined in swArrowStyle\_e

*EndPointArrowStyle*
:   Ending point's arrowhead style as defined in  swArrowStyle\_e

#### Return Value

Newly created multi-jog leader

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertMultiJogLeader3.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::IInsertMultiJogLeader3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IInsertMultiJogLeader3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0