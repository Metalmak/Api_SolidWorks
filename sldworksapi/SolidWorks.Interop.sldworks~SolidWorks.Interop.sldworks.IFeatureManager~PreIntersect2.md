<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PreIntersect2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PreIntersect2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : PreIntersect2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CapPlanar*
:   True to cap the flat openings of surfaces to define closed volumes, false to not

*RegionType*
:   Type of regions to create:

    * 0 = Intersecting regions* 1 = Internal regions* 2 = Intersecting and internal regions

Prepares an intersect feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PreIntersect2( _    ByVal CapPlanar As System.Boolean, _    ByVal RegionType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim CapPlanar As System.Boolean Dim RegionType As System.Integer Dim value As System.Object   value = instance.PreIntersect2(CapPlanar, RegionType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object PreIntersect2(     System.bool CapPlanar,    System.int RegionType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ PreIntersect2(  &   System.bool CapPlanar, &   System.int RegionType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CapPlanar*
:   True to cap the flat openings of surfaces to define closed volumes, false to not

*RegionType*
:   Type of regions to create:

    * 0 = Intersecting regions* 1 = Internal regions* 2 = Intersecting and internal regions

#### Return Value

Array of intersecting [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::PreIntersect2.

# ![](dotnetimages/collapse.gif)Example

[Create Intersect Feature (C#)](Create_Intersect_Feature_Example_CSharp.htm)

[Create Intersect Feature (VB.NET)](Create_Intersect_Feature_Example_VBNET.htm)

[Create Intersect Feature (VBA)](Create_Intersect_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must select the intersecting [surfaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html), [solids](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html), or [planes](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html) that make up the intersect feature.

After calling this method, call [IFeatureManager::PostIntersect](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~PostIntersect.html) to create the intersect feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IIntersectFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIntersectFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0