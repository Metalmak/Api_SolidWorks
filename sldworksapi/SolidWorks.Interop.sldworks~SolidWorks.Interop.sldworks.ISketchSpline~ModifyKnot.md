<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ModifyKnot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModifyKnot Method (ISketchSpline) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html) : ModifyKnot Method (ISketchSpline) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   1-based index of the interior knot to modify (see **Remarks**)

*DKnot*
:   Knot value

Modifies the specified interior knot of this sketch spline.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ModifyKnot( _    ByVal Index As System.Integer, _    ByVal DKnot As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSpline Dim Index As System.Integer Dim DKnot As System.Double Dim value As System.Boolean   value = instance.ModifyKnot(Index, DKnot) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ModifyKnot(     System.int Index,    System.double DKnot ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ModifyKnot(  &   System.int Index, &   System.double DKnot ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   1-based index of the interior knot to modify (see **Remarks**)

*DKnot*
:   Knot value

#### Return Value

True if knot successfully modifed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSpline::ModifyKnot.

# ![](dotnetimages/collapse.gif)Example

[Edit Spline (VBA)](Edit_Spline_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Interior knots occur after the first set of 0s and before the last set of 1s in the knot array. If the knot array is [ 0 0 0 0 0.279240779943874 0.55 0.720759220056126 1 1 1 1 ], then the interior knots are 0.279240779943874, 0.55, and 0.720759220056126.

Before calling this method, call [ISplineParamData::GetKnotPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplineParamData~GetKnotPoints.html) and [ISplineParamData::KnotPointsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplineParamData~KnotPointsCount.html) to help specify Index and the new knot value.

After calling this method, you must call [IModelDoc2::ForceRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ForceRebuild3.html) to update the sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html)

[ISketchSpline Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline_members.html)

[ISketchSpline::ModifyControlPoint Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~ModifyControlPoint.html)

[ISplineParamData::SetKnotPoints Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplineParamData~SetKnotPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0