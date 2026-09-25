<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane~CornerPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CornerPoints Property (IRefPlane) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) : CornerPoints Property (IRefPlane) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the corner points of this reference plane.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property CornerPoints As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRefPlane Dim value As System.Object   value = instance.CornerPoints ``` | |

| C# |  |
| --- | --- |
| ``` System.object CornerPoints {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ CornerPoints {    System.Object^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of four (4) [IMathpoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) objects

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RefPlane::CornerPoints.

# ![](dotnetimages/collapse.gif)Example

[Get Corner Points of Reference Plane (VBA)](Get_Corner_Points_of_Reference_Plane_Example_VB.htm)

[Get Corner Points of Reference Plane (VB.NET)](Get_Corner_Points_of_Reference_Plane_Example_VBNET.htm)

[Get Corner Points of Reference Plane (C#)](Get_Corner_Points_of_Reference_Plane_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html)

[IRefPlane Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane_members.html)

[IRefPlane::IGetCornerPoints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane~IGetCornerPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP5, Revision Number 17.5