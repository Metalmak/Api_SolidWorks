<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetBreakLineInfo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetBreakLineInfo2 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetBreakLineInfo2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArraySize*
:   Number of break lines

Gets information for all of the break lines in this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetBreakLineInfo2( _    ByVal ArraySize As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim ArraySize As System.Integer Dim value As System.Double   value = instance.IGetBreakLineInfo2(ArraySize) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetBreakLineInfo2(     System.int ArraySize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetBreakLineInfo2(  &   System.int ArraySize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArraySize*
:   Number of break lines

#### Return Value

* in-process, unmanaged C++: Pointer to an array of break line information (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IView::GetBreakLineCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetBreakLineCount2.html) to get the value for ArraySize.

The return value is a one-dimensional array consisting of the following data:

[ breaklineStyle, color, lineType, lineStyleIndex, lineWeight, layerId,

    layerOverride, numLines, numArcs, numSplines, [break line data] ]

where:

|  |  |
| --- | --- |
| breaklineStyle | Break line style as defined in swBreakLineStyle\_e |
| color | COLORREF returned as an integer; 0 or -1 for default color |
| lineType | Line type as defined in swLineTypes\_e; lineType is a combination of a lineStyle and lineWeight |
| lineStyleIndex | Line style as defined in swLineStyles\_e |
| lineWeight | Line width as defined in swLineWeights\_e |
| layerId | An integer value indicating which layer holds this entity; [ILayer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayer.html) can be obtained by passing this integer value to [ILayerMgr::GetLayerById](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~GetLayerById.html) and [ILayerMgr::IGetLayerId](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILayerMgr~IGetLayerById.html) |
| layerOverride | An integer with bit flags set to determine which properties, if any, have been overridden with respect to the Layer default properties. If the bit value is set, then the specific property or properties have been overridden. Valid bit values as defined in swLayerOverride\_e:   * color = 0x1 * style = 0x2 * width = 0x4   Therefore, if LayerOverride is returned as 3, then the color and style are specifically set for this item and may not match the default values associated with this item's layer. |
| *numLines* | Number of line segments if a straight or zig zag break |
| *numArcs* | Number of arc lines if a curve break |
| *numSplines* | Number of spline lines if a jagged break |

|  |  |
| --- | --- |
| **If the break line style is swBreakLineStyle\_e...** | **Then [ *break line data* ] is packed with...** |
| swBreakLine\_Straight | 12 doubles (2 lines \* 1 segment \* 2 points \* 3 coordinates) |
| swBreakLine\_ZigZag | 60 doubles (2 lines \* 5 segments \* 2 points \* 3 coordinates) |
| swBreakLine\_SmallZigZag | 60 doubles (2 lines \* 5 segments \* 2 points \* 3 coordinates) |
| swBreakLine\_Curve | for each arc line in the break:   * arc direction (1 double) * start point (3 doubles) * end point (3 doubles) * center point (3 doubles) |
| swBreakLine\_Jagged | for each spline line in the break:   * *n* (1 integer)* 3\**n* doubles (*n* points \* 3 coordinates)   where:  *n* is the number of spline points generated based on the jagged cut shape intensity selected by the user in the Break View Property Manager |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetBreakLineInfo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineInfo2.html)

[IView::GetBreakLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLines.html)

[IView::IGetBreakLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetBreakLines.html)

[IView::IsBroken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsBroken.html)

[IView::BreakLineGap Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~BreakLineGap.html)

[IView::InsertBreak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBreak.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0