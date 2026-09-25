<!-- source: swscanto3dapi/SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Scanto3D API Help | Send comments on this topic. |
| IScanto3D Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swscanto3d Namespace](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d_namespace.html) : IScanto3D Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to Scanto3D point cloud data.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IScanto3D ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IScanto3D ``` | |

| C# |  |
| --- | --- |
| ``` public interface IScanto3D ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IScanto3D ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Scanto3D.

# ![](dotnetimages/collapse.gif)Example

[Get Mesh Data (VBA)](Get_Mesh_Data_Example_VB.htm)

[Get Mesh Data (VB.NET)](Get_Mesh_Data_Example_VBNET.htm)

[Get Mesh Data (C#)](Get_Mesh_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To obtain the data for the entire mesh:

1. Call [IScanto3D::GetMeshCount](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshCount.html) to get the number of mesh features, *n*.- Call [IScanto3D::GetMeshDataCountAtIndex](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshDataCountAtIndex.html) iteratively *n* times to get the number of points and facets in each mesh feature.- Call [IScanto3D::GetMeshDataAtIndex](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D~GetMeshDataAtIndex.html) iteratively *n* times to get the data in each mesh feature.

# ![](dotnetimages/collapse.gif)Accessors

IModelDocExtension::GetScanto3D

# ![](dotnetimages/collapse.gif)See Also

####

[IScanto3D Members](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d.IScanto3D_members.html)

[SolidWorks.Interop.swscanto3d Namespace](SolidWorks.Interop.swscanto3d~SolidWorks.Interop.swscanto3d_namespace.html)