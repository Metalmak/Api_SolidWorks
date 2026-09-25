<!-- source: swscanto3dapi/SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshDataAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Scanto3D API Help | Send comments on this topic. |
| GetMeshDataAtIndex Method (IScanto3D) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swscanto3d Namespace](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d_namespace.html) > [IScanto3D Interface](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html) : GetMeshDataAtIndex Method (IScanto3D) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of mesh feature for which to get data

*Points*
:   Array of x, y, and z coordinates of the mesh vertexes (see **Remarks**)

*Facets*
:   Array of facet triplets (see **Remarks**)

Gets the points and facets in the specified mesh feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMeshDataAtIndex( _    ByVal Index As System.Integer, _    ByRef Points As System.Object, _    ByRef Facets As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IScanto3D Dim Index As System.Integer Dim Points As System.Object Dim Facets As System.Object Dim value As System.Boolean   value = instance.GetMeshDataAtIndex(Index, Points, Facets) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetMeshDataAtIndex(     System.int Index,    out System.object Points,    out System.object Facets ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetMeshDataAtIndex(  &   System.int Index, &   [Out] System.Object^ Points, &   [Out] System.Object^ Facets ) ``` | |

#### Parameters

*Index*
:   Index of mesh feature for which to get data

*Points*
:   Array of x, y, and z coordinates of the mesh vertexes (see **Remarks**)

*Facets*
:   Array of facet triplets (see **Remarks**)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Scanto3D::GetMeshDataAtIndex.

# ![](dotnetimages/collapse.gif)Example

See the [IScanto3D](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IScanto3D::GetMeshCount](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshCount.html) to obtain the total number of mesh features in this mesh.

Each facet in the mesh can be described by a triangle consisting of three mesh vertexes. Adjacent facets share their vertexes.

For example, if this method returns in Points a 0-based array of the coordinates of each vertex of a mesh feature specified by Index:

[

pt1x, pt1y, pt1z,

pt2x, t2y, pt2z,

pt3x, pt3y, pt3z,

pt4x, pt4y, pt4z,

pt5x, pt5y, pt5z,

pt6x, pt6y, pt6z

...

],

then it also returns in Facets an array of triplets of integers that are indexes into the array returned in Points:

[

{pt1x\_idx, pt2\_idx, pt3\_idx},

{pt6\_idx, pt4\_idx, pt1\_idx},

...

],

where the first facet is {0, 3, 6}, i.e.,  (pt1\_idx = 0, pt2\_idx = 3, pt3\_idx = 6),

and the second facet is {15, 9, 0}, i.e.,  (pt6\_idx = 15, pt4\_idx = 9, pt1\_idx = 0).

# ![](dotnetimages/collapse.gif)See Also

####

[IScanto3D Interface](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html)

[IScanto3D Members](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0