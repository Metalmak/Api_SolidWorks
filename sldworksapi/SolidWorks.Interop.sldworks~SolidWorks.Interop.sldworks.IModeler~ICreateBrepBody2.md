<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBrepBody2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBrepBody2 Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateBrepBody2 Method (IModeler) |

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

*EdgeTolArray*

*VertexTolArray*

*PointArray*

*CurveArray*

*SurfaceArray*

*NRelations*

*Parents*

*Children*

*Senses*

Obsolete. Superseded by [IModeler::ICreateBrepBody3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICreateBrepBody3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBrepBody2( _    ByVal Type As System.Integer, _    ByVal NTopologies As System.Integer, _    ByRef Topologies As System.Integer, _    ByRef EdgeTolArray As System.Double, _    ByRef VertexTolArray As System.Double, _    ByRef PointArray As System.Double, _    ByRef CurveArray As Curve, _    ByRef SurfaceArray As Surface, _    ByVal NRelations As System.Integer, _    ByRef Parents As System.Integer, _    ByRef Children As System.Integer, _    ByRef Senses As System.Integer _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Type As System.Integer Dim NTopologies As System.Integer Dim Topologies As System.Integer Dim EdgeTolArray As System.Double Dim VertexTolArray As System.Double Dim PointArray As System.Double Dim CurveArray As Curve Dim SurfaceArray As Surface Dim NRelations As System.Integer Dim Parents As System.Integer Dim Children As System.Integer Dim Senses As System.Integer Dim value As Body2   value = instance.ICreateBrepBody2(Type, NTopologies, Topologies, EdgeTolArray, VertexTolArray, PointArray, CurveArray, SurfaceArray, NRelations, Parents, Children, Senses) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 ICreateBrepBody2(     System.int Type,    System.int NTopologies,    ref System.int Topologies,    ref System.double EdgeTolArray,    ref System.double VertexTolArray,    ref System.double PointArray,    ref Curve CurveArray,    ref Surface SurfaceArray,    System.int NRelations,    ref System.int Parents,    ref System.int Children,    ref System.int Senses ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ ICreateBrepBody2(  &   System.int Type, &   System.int NTopologies, &   System.int% Topologies, &   System.double% EdgeTolArray, &   System.double% VertexTolArray, &   System.double% PointArray, &   Curve^% CurveArray, &   Surface^% SurfaceArray, &   System.int NRelations, &   System.int% Parents, &   System.int% Children, &   System.int% Senses ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*

*NTopologies*

*Topologies*

*EdgeTolArray*

*VertexTolArray*

*PointArray*

*CurveArray*

*SurfaceArray*

*NRelations*

*Parents*

*Children*

*Senses*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICreateBrepBody2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)