<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDiamDim4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateDiamDim4 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateDiamDim4 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*P0*
:   Pointer to an array of 3 doubles (x,y,z); location of dimension point

*P1*
:   Pointer to an array of 3 doubles (x,y,z); nearest point on circle

*P2*
:   Pointer to an array of 3 doubles (x,y,z); farthest point on circle diametrically opposite to P1

*P3*
:   Pointer to an array of 3 doubles (x,y,z); plane normal

*TextPoint*
:   Pointer to an array of 3 doubles (x,y,z); position of text

*Val*
:   Dimension value in meters

*TextHeight*
:   Text height in meters

Creates a non-associative diameter dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateDiamDim4( _    ByRef P0 As System.Double, _    ByRef P1 As System.Double, _    ByRef P2 As System.Double, _    ByRef P3 As System.Double, _    ByRef TextPoint As System.Double, _    ByVal Val As System.Double, _    ByVal TextHeight As System.Double _ ) As DisplayDimension ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim P0 As System.Double Dim P1 As System.Double Dim P2 As System.Double Dim P3 As System.Double Dim TextPoint As System.Double Dim Val As System.Double Dim TextHeight As System.Double Dim value As DisplayDimension   value = instance.ICreateDiamDim4(P0, P1, P2, P3, TextPoint, Val, TextHeight) ``` | |

| C# |  |
| --- | --- |
| ``` DisplayDimension ICreateDiamDim4(     ref System.double P0,    ref System.double P1,    ref System.double P2,    ref System.double P3,    ref System.double TextPoint,    System.double Val,    System.double TextHeight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DisplayDimension^ ICreateDiamDim4(  &   System.double% P0, &   System.double% P1, &   System.double% P2, &   System.double% P3, &   System.double% TextPoint, &   System.double Val, &   System.double TextHeight ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*P0*
:   Pointer to an array of 3 doubles (x,y,z); location of dimension point

*P1*
:   Pointer to an array of 3 doubles (x,y,z); nearest point on circle

*P2*
:   Pointer to an array of 3 doubles (x,y,z); farthest point on circle diametrically opposite to P1

*P3*
:   Pointer to an array of 3 doubles (x,y,z); plane normal

*TextPoint*
:   Pointer to an array of 3 doubles (x,y,z); position of text

*Val*
:   Dimension value in meters

*TextHeight*
:   Text height in meters

#### Return Value

Pointer to the new [IDisplayDimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateDiamDim4.

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS creates this type of dimension between the two points you specify. It has no relation to your geometry.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::CreateLinearDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateLinearDim4.html)

[IDrawingDoc::CreateDiamDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDiamDim4.html)

[IDrawingDoc::CreateOrdinateDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateOrdinateDim4.html)

[IDrawingDoc::ICreateDiamDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDiamDim4.html)

[IDrawingDoc::ICreateLinearDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateLinearDim4.html)

[IDrawingDoc::ICreateOrdinateDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateOrdinateDim4.html)

[IDrawingDoc::ICreateAngDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateAngDim4.html)

[IDrawingDoc::CreateAngDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateAngDim4.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0