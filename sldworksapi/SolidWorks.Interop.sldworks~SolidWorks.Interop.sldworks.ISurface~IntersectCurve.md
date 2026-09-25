<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IntersectCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IntersectCurve Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IntersectCurve Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OtherCurve*

*CurveBound*

*PointArray*

*TArray*

*UvArray*

Obsolete. Superseded by [ISurface::IntersectCurve2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IIntersectCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IntersectCurve( _    ByVal OtherCurve As System.Object, _    ByVal CurveBound As System.Object, _    ByRef PointArray As System.Object, _    ByRef TArray As System.Object, _    ByRef UvArray As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim OtherCurve As System.Object Dim CurveBound As System.Object Dim PointArray As System.Object Dim TArray As System.Object Dim UvArray As System.Object Dim value As System.Boolean   value = instance.IntersectCurve(OtherCurve, CurveBound, PointArray, TArray, UvArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IntersectCurve(     System.object OtherCurve,    System.object CurveBound,    out System.object PointArray,    out System.object TArray,    out System.object UvArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IntersectCurve(  &   System.Object^ OtherCurve, &   System.Object^ CurveBound, &   [Out] System.Object^ PointArray, &   [Out] System.Object^ TArray, &   [Out] System.Object^ UvArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OtherCurve*

*CurveBound*

*PointArray*

*TArray*

*UvArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IntersectCurve.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)