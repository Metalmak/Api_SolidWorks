<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreatePlanarTrimSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreatePlanarTrimSurfaceDLL Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : CreatePlanarTrimSurfaceDLL Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Points*
:   Array of the points for the surface; trim curves are automatically created between each sequential vertex

*Normal*
:   Array of normal vector for the surface

Creates a planar trim surface for this body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePlanarTrimSurfaceDLL( _    ByVal Points As System.Object, _    ByVal Normal As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Points As System.Object Dim Normal As System.Object Dim value As System.Boolean   value = instance.CreatePlanarTrimSurfaceDLL(Points, Normal) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreatePlanarTrimSurfaceDLL(     System.object Points,    System.object Normal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreatePlanarTrimSurfaceDLL(  &   System.Object^ Points, &   System.Object^ Normal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Points*
:   Array of the points for the surface; trim curves are automatically created between each sequential vertex

*Normal*
:   Array of normal vector for the surface

#### Return Value

True if planar trim surface is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::CreatePlanarTrimSurfaceDLL.

# ![](dotnetimages/collapse.gif)Example

[Create Imported Solid Body (C#)](Create_Imported_Solid_Body_Example_CSharp.htm)

[Create Imported Solid Body (VB.NET)](Create_Imported_Solid_Body_Example_VBNET.htm)

[Create Imported Solid Body (VBA)](Create_Imported_Solid_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method instead of [IBody2:CreateTrimmedSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateTrimmedSurface.html), [IBody2::ICreatePlanarSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreatePlanarSurface.html), and [ISurface::AddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~AddTrimmingLoop2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::ICreatePlanarTrimSurfaceDLL Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePlanarTrimSurfaceDLL.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP1, Revision Number 12