<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreatePlanarSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreatePlanarSurface Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : CreatePlanarSurface Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VRootPoint*
:   Array of 3 doubles (x,y,z)

*VNormal*
:   Array of 3 doubles (x,y,z)

Creates a new infinite planar surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePlanarSurface( _    ByVal VRootPoint As System.Object, _    ByVal VNormal As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim VRootPoint As System.Object Dim VNormal As System.Object Dim value As System.Object   value = instance.CreatePlanarSurface(VRootPoint, VNormal) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreatePlanarSurface(     System.object VRootPoint,    System.object VNormal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreatePlanarSurface(  &   System.Object^ VRootPoint, &   System.Object^ VNormal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VRootPoint*
:   Array of 3 doubles (x,y,z)

*VNormal*
:   Array of 3 doubles (x,y,z)

#### Return Value

New planar surface

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::CreatePlanarSurface.

# ![](dotnetimages/collapse.gif)Example

[Create Body Using Trimmed Surfaces (VBA)](Create_Body_using_Trimmed_Surfaces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with:

* A set of related functions that construct a body from trimmed surfaces.

  * Trimming curve creation routines (for example, [ISurface::AddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~AddTrimmingLoop2.html)) to construct a trimmed surface.

To create a planar trimmed surface directly from the vertex points, see [IBody2::CreatePlanarTrimSurfaceDLL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreatePlanarTrimSurfaceDLL.html).

Any existing object created by this method is destroyed if you call this method again.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::ICreatePlanarSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePlanarSurface.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0