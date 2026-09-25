<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetBCurveParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBCurveParams Method (ICurve) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : GetBCurveParams Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WantCubicIn*
:   True returns cubic rational parameters, false does not

Obsolete. Superseded by [ICurve::GetBCurveParams3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetBCurveParams3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBCurveParams( _    ByVal WantCubicIn As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim WantCubicIn As System.Boolean Dim value As System.Object   value = instance.GetBCurveParams(WantCubicIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBCurveParams(     System.bool WantCubicIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBCurveParams(  &   System.bool WantCubicIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WantCubicIn*
:   True returns cubic rational parameters, false does not

#### Return Value

Array describing the parameters of the curve (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::GetBCurveParams.

# ![](dotnetimages/collapse.gif)Example

[Get Curve Spline Points (VBA)](Get_Curve_Spline_Points_Example_VB.htm)

[Select Edges of All Holes on Face (C#)](Select_Edges_of_All_Holes_on_Face_Example_CSharp.htm)

[Select Edges of All Holes on Face (VB.NET)](Select_Edges_of_All_Holes_on_Face_Example_VBNET.htm)

[Select Edges of All Holes on Face (VBA)](Select_Edges_of_All_Holes_on_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To control the accuracy of the curve data, see [IModeler::SetToleranceValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~SetToleranceValue.html).

The return value is an array of doubles. The array size is ( 2 + numKnots + numControlPointDoubles) where numKnots is (numControlPoints + order). The array is as follows:

**[** *packedDouble1, packedDouble2, knot1, knot2,..., ControlPoint1[Dimension], ControlPoint2[Dimension],...***]**

where:

* *packedDouble1* is an integer pair containing the *Dimension* and *Order** *packedDouble2*  is an integer pair containing the *NumControlPoints* and *Periodicity** *knot1** *knot2*

...

* *ControlPoint1[dimension]** *ControlPoint2[dimension]*

...

The size of the control point array is based on the curve dimension:

* If *Dimension* = 3, then *ControlPoint* is an array of 3 doubles ( x, y, z )* If *Dimension* = 4, then *ControlPoint* is an array of 4 doubles ( x, y, z, w ) where
    w = weight

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::ConvertArcToBcurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertArcToBcurve.html)

[ICurve::ConvertLineToBcurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ConvertLineToBcurve.html)

[ICurve::IGetBCurveParamsSize2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetBCurveParamsSize2.html)

[ICurve::ICurve::IsBcurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IsBcurve.html)

[ICurve::IConvertPcurveToBcurveSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IConvertPcurveToBcurveSize.html)

[ICurve::SimplifyBCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~SimplifyBCurve.html)