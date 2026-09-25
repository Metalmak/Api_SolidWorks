<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~EvaluateAtPoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EvaluateAtPoint Method (ISurface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : EvaluateAtPoint Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PositionX*
:   X position

*PositionY*
:   Y position

*PositionZ*
:   Z position

Evaluates a surface at the specified XYZ point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EvaluateAtPoint( _    ByVal PositionX As System.Double, _    ByVal PositionY As System.Double, _    ByVal PositionZ As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim PositionX As System.Double Dim PositionY As System.Double Dim PositionZ As System.Double Dim value As System.Object   value = instance.EvaluateAtPoint(PositionX, PositionY, PositionZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.object EvaluateAtPoint(     System.double PositionX,    System.double PositionY,    System.double PositionZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ EvaluateAtPoint(  &   System.double PositionX, &   System.double PositionY, &   System.double PositionZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PositionX*
:   X position

*PositionY*
:   Y position

*PositionZ*
:   Z position

#### Return Value

Array of doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::EvaluateAtPoint.

# ![](dotnetimages/collapse.gif)Example

[Determine Type of Face (VBA)](Determine_Type_of_Face_Example_VB.htm)

[Evaluate Points on Surface (VBA)](Evaluate_Points_on_Surface_Example_VB.htm)

[Select Tangent Faces (VBA)](Select_Tangent_Faces_Example_VB.htm)

[Select Edges of All Holes on Face (C#)](Select_Edges_of_All_Holes_on_Face_Example_CSharp.htm)

[Select Edges of All Holes on Face (VB.NET)](Select_Edges_of_All_Holes_on_Face_Example_VBNET.htm)

[Select Edges of All Holes on Face (VBA)](Select_Edges_of_All_Holes_on_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method calculates the normal, the principal directions, and the principal curvatures, of the surface at the specified point.

Use [IFace2::FaceInSurfaceSense](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~FaceInSurfaceSense.html) to check the directions of the face normal and surface normal. IFace2::FaceInSurfaceSense returns true when the face normal and surface normal point in opposite directions, and false when they point in the same direction.

The return value is the following array of eleven doubles:

[surfNorm[i, j, k], principalDir1[i, j, k], principalDir2[I, j, k], principalCurvature1, principalCurvature2 ]

where:

surfNorm[i, j, k] = normalized vector describing the surface normal

principalDir1[i, j, k] = normalized vector describing the first principal direction

principalDir2[i, j, k] = normalized vector describing the second principal direction

principalCurvature1 = first principal curvature

principalCurvature2 = second principal curvature

Principal Curvature 1 is the minimum normal curvature at the point (largest radius). Principal Curvature 2 is the maximum normal curvature at the point.

The tangent direction producing Principal Curvature 1 is called the first principal direction, and the tangent direction producing Principal Curvature 2 is called the second principal direction.

It is a property of differentiable surfaces that principalDir1 and principalDir2 are orthogonal.

A positive curvature by convention implies a centre of curvature on the side pointed away from by the surface normal (convex).

See "Faux and Pratt Computational Geometry for Design and Manufacture" for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IEvaluateAtPoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IEvaluateAtPoint.html)

[ISurface::IEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IEvaluate.html)

[ISurface::Evaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~Evaluate.html)

[ISurface::IParameterization Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IParameterization.html)

[ISurface::IReverseEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IReverseEvaluate.html)

[ISurface::Parameterization Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~Parameterization.html)

[ISurface::ReverseEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~ReverseEvaluate.html)