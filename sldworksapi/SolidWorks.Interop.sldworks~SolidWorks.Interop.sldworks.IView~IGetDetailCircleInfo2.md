<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDetailCircleInfo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetDetailCircleInfo2 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetDetailCircleInfo2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArraySize*
:   Extra double for each detail circle; this array entity contains the layer ID for the detail circle, and it is the first entity in the array for each detail circle (see Remarks)

Gets all of the information about each detail circle in the view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetDetailCircleInfo2( _    ByVal ArraySize As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim ArraySize As System.Integer Dim value As System.Double   value = instance.IGetDetailCircleInfo2(ArraySize) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetDetailCircleInfo2(     System.int ArraySize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetDetailCircleInfo2(  &   System.int ArraySize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArraySize*
:   Extra double for each detail circle; this array entity contains the layer ID for the detail circle, and it is the first entity in the array for each detail circle (see Remarks)

#### Return Value

Array of doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::IGetDetailCircleInfo2.

# ![](dotnetimages/collapse.gif)Remarks

The return value is the following array of doubles:

[ numDetailCircles, [ layer, centerPt[3], startPt[3], endPt[3], lineType, textPt[3], textHeight, numArrows, [ arrowTip[3], arrowComponent[3], arrowWidth, arrowHeight, arrowStyle ] ] ]

where:

numDetailCircles = the number of detail circles in this view. See also [IView::GetDetailCircleCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetDetailCircleCount2.html).

The following set of data repeats itself for each detail circle in the view. The number of times the following information is given is numDetailCircles:

layer = integer value indicating which layer holds this entity. Obtain the [ILayer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayer.html) object by passing this integer value to [ILayerMgr::GetLayerById](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~GetLayerById.html) or [ILayerMgr::IGetLayerById](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~IGetLayerById.html).

centerPt[3] = X,Y,Z center point for this detail circle

startPt[3] = X,Y,Z start point for this detail circle

endPt[3] = X,Y,Z end point for this detail circle

lineType  = line type for this detail circle as defined in swLineTypes\_e

textPt[3] = X,Y,Z point for the text location.

textHeight  = text height in meters

numArrows = number of arrows for this detail circle.

The following set of data repeats itself for each arrow in the current detail circle. The number of times the following information is given is numArrows:

arrowTip[3]  = X,Y,Z start point for this arrow head

arrowComponent[3]  = X,Y,Z component for this arrow head

arrowWidth = width of this arrow head

arrowHeight = height of this arrow head

arrowStyle = style of this arrow head as defined in swArrowStyle\_e

To get the actual text value, see [IView::GetDetailCircleStrings](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetDetailCircleStrings.html) or [IView::IGetDetailCircleStrings](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetDetailCircleStrings.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IGetDetail Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDetail.html)

[IView::IGetDetailCircles Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDetailCircles.html)

[IView::GetDetail Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDetail.html)

[IView::GetDetailCircleInfo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDetailCircleInfo2.html)

[IView::GetDetailCircles Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDetailCircles.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0