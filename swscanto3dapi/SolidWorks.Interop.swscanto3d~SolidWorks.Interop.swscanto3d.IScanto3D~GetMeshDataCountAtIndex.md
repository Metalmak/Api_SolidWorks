<!-- source: swscanto3dapi/SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshDataCountAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Scanto3D API Help | Send comments on this topic. |
| GetMeshDataCountAtIndex Method (IScanto3D) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swscanto3d Namespace](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d_namespace.html) > [IScanto3D Interface](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html) : GetMeshDataCountAtIndex Method (IScanto3D) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of mesh feature for which to get data

*PointsCount*
:   Number of points in the mesh at Index

*FacetsCount*
:   Number of facets in the mesh at Index

Gets the number of points and facets in the specified mesh feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMeshDataCountAtIndex( _    ByVal Index As System.Integer, _    ByRef PointsCount As System.Integer, _    ByRef FacetsCount As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IScanto3D Dim Index As System.Integer Dim PointsCount As System.Integer Dim FacetsCount As System.Integer Dim value As System.Boolean   value = instance.GetMeshDataCountAtIndex(Index, PointsCount, FacetsCount) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetMeshDataCountAtIndex(     System.int Index,    out System.int PointsCount,    out System.int FacetsCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetMeshDataCountAtIndex(  &   System.int Index, &   [Out] System.int PointsCount, &   [Out] System.int FacetsCount ) ``` | |

#### Parameters

*Index*
:   Index of mesh feature for which to get data

*PointsCount*
:   Number of points in the mesh at Index

*FacetsCount*
:   Number of facets in the mesh at Index

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Scanto3D::GetMeshDataCountAtIndex.

# ![](dotnetimages/collapse.gif)Example

See the [IScanto3D](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IScanto3D::GetMeshCount](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshCount.html) to obtain the total number of mesh features in this mesh.

# ![](dotnetimages/collapse.gif)See Also

####

[IScanto3D Interface](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html)

[IScanto3D Members](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0