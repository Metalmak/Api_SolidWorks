<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetDefaultMaxAndMinElementSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetDefaultMaxAndMinElementSize Method (ICWMesh) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetDefaultMaxAndMinElementSize Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUnits*
:   Mesh linear units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DMaxElementSize*
:   Maximum element size used for boundaries with lowest curvature

*DMinElementSize*
:   Minimum element size used for boundaries with highest curvature

Gets the default maximum and minimum element sizes used for boundaries in a curvature-based mesh.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetDefaultMaxAndMinElementSize( _    ByVal NUnits As System.Integer, _    ByRef DMaxElementSize As System.Double, _    ByRef DMinElementSize As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim NUnits As System.Integer Dim DMaxElementSize As System.Double Dim DMinElementSize As System.Double   instance.GetDefaultMaxAndMinElementSize(NUnits, DMaxElementSize, DMinElementSize) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDefaultMaxAndMinElementSize(     System.int NUnits,    out System.double DMaxElementSize,    out System.double DMinElementSize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDefaultMaxAndMinElementSize(  &   System.int NUnits, &   [Out] System.double DMaxElementSize, &   [Out] System.double DMinElementSize ) ``` | |

#### Parameters

*NUnits*
:   Mesh linear units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DMaxElementSize*
:   Maximum element size used for boundaries with lowest curvature

*DMinElementSize*
:   Minimum element size used for boundaries with highest curvature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetDefaultMaxAndMinElementSize.

# ![](dotnetimages/collapse.gif)Example

[Create Curvature-based Mesh (C#)](Create_Curvature-based_Mesh_Example_CSharp.htm)

[Create Curvature-based Mesh (VB.NET)](Create_Curvature-based_Mesh_Example_VBNET.htm)

[Create Curvature-based Mesh (VBA)](Create_Curvature-based_Mesh_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GrowthRatio Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GrowthRatio.html)

[ICWMesh::MaxElementSize Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MaxElementSize.html)

[ICWMesh::MinElementSize Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MinElementSize.html)

[ICWMesh::MinElementsInCircle Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MinElementsInCircle.html)

[ICWMesh::MesherType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MesherType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2011 SP0