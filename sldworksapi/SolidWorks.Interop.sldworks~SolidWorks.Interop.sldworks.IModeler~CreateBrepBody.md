<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateBrepBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateBrepBody Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CreateBrepBody Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*

*NTopologies*

*Topologies*

*EdgeToleranceArray*

*VertexToleranceArray*

*PointArray*

*CurveArray*

*SurfaceArray*

*NRelations*

*Parents*

*Children*

*Senses*

Obsolete. Superseded by [IModeler::CreateBrepBody3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~CreateBrepBody3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateBrepBody( _    ByVal Type As System.Integer, _    ByVal NTopologies As System.Integer, _    ByVal Topologies As System.Object, _    ByVal EdgeToleranceArray As System.Object, _    ByVal VertexToleranceArray As System.Object, _    ByVal PointArray As System.Object, _    ByVal CurveArray As System.Object, _    ByVal SurfaceArray As System.Object, _    ByVal NRelations As System.Integer, _    ByVal Parents As System.Object, _    ByVal Children As System.Object, _    ByVal Senses As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Type As System.Integer Dim NTopologies As System.Integer Dim Topologies As System.Object Dim EdgeToleranceArray As System.Object Dim VertexToleranceArray As System.Object Dim PointArray As System.Object Dim CurveArray As System.Object Dim SurfaceArray As System.Object Dim NRelations As System.Integer Dim Parents As System.Object Dim Children As System.Object Dim Senses As System.Object Dim value As System.Object   value = instance.CreateBrepBody(Type, NTopologies, Topologies, EdgeToleranceArray, VertexToleranceArray, PointArray, CurveArray, SurfaceArray, NRelations, Parents, Children, Senses) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateBrepBody(     System.int Type,    System.int NTopologies,    System.object Topologies,    System.object EdgeToleranceArray,    System.object VertexToleranceArray,    System.object PointArray,    System.object CurveArray,    System.object SurfaceArray,    System.int NRelations,    System.object Parents,    System.object Children,    System.object Senses ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateBrepBody(  &   System.int Type, &   System.int NTopologies, &   System.Object^ Topologies, &   System.Object^ EdgeToleranceArray, &   System.Object^ VertexToleranceArray, &   System.Object^ PointArray, &   System.Object^ CurveArray, &   System.Object^ SurfaceArray, &   System.int NRelations, &   System.Object^ Parents, &   System.Object^ Children, &   System.Object^ Senses ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*

*NTopologies*

*Topologies*

*EdgeToleranceArray*

*VertexToleranceArray*

*PointArray*

*CurveArray*

*SurfaceArray*

*NRelations*

*Parents*

*Children*

*Senses*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CreateBrepBody.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)