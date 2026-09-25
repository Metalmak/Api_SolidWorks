<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane~BoundingBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| BoundingBox Property (IRefPlane) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) : BoundingBox Property (IRefPlane) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the bounding box of the reference plane, the top-left and bottom-right points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property BoundingBox As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRefPlane Dim value As System.Object   value = instance.BoundingBox ``` | |

| C# |  |
| --- | --- |
| ``` System.object BoundingBox {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ BoundingBox {    System.Object^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array containing bounding box, always two (2) [IMathpoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) objects

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RefPlane::BoundingBox.

# ![](dotnetimages/collapse.gif)Example

[Get Coordinates of the Plane's Bounding Box (C#)](Get_Coordinates_of_the_Plane%27s_Bounding_Box_Example_CSharp.htm)

[Get Coordinates of the Plane's Bounding Box (VB.NET)](Get_Coordinates_of_the_Plane%27s_Bounding_Box_Example_VBNET.htm)

[Get Coordinates of the Plane's Bounding Box (VBA)](Get_Coordinates_of_the_Plane%27s_Bounding_Box_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html)

[IRefPlane Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane_members.html)

[IRefPlane::IGetBoundingBox Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane~IGetBoundingBox.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0