<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~Insert3DSplineCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Insert3DSplineCurve Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : Insert3DSplineCurve Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CurveClosed*
:   True if you want the curve to be closed, false if not

Inserts a 3D-spline curve through the selected reference points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Insert3DSplineCurve( _    ByVal CurveClosed As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim CurveClosed As System.Boolean   instance.Insert3DSplineCurve(CurveClosed) ``` | |

| C# |  |
| --- | --- |
| ``` void Insert3DSplineCurve(     System.bool CurveClosed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Insert3DSplineCurve(  &   System.bool CurveClosed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CurveClosed*
:   True if you want the curve to be closed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::Insert3DSplineCurve.

# ![](dotnetimages/collapse.gif)Example

[Insert a 3D-Spline Curve (VBA)](Insert_3D_Spline_Curve_Example_VB.htm)

[Create Curve Through Reference Points (VBA)](Create_Curve_Through_Reference_Points_Example_VB.htm)

[Create Curve Through Reference Points (VB.NET)](Create_Curve_Through_Reference_Points_Example_VBNET.htm)

[Create Curve Through Reference Points (C#)](Create_Curve_Through_Reference_Points_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select the reference points by calling [IModelDocExtension::SelectbyID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Marks of 1.

To create 2D splines on a sketch, use [IModelDoc2::SketchSpline](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SketchSpline.html) or [IModelDoc2::CreateSpline](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateSpline.html) or [IModelDoc2::ICreateSpline](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ICreateSpline.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0