<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~IAddProfileBsplineDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddProfileBsplineDLL Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : IAddProfileBsplineDLL Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Properties*

*KnotArray*

*ControlPointCoordArray*

Obsolete. Superseded by [IBody2::IAddProfileBsplineDLL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IAddProfileBsplineDLL.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddProfileBsplineDLL( _    ByRef Properties As System.Integer, _    ByRef KnotArray As System.Double, _    ByRef ControlPointCoordArray As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Properties As System.Integer Dim KnotArray As System.Double Dim ControlPointCoordArray As System.Double Dim value As Curve   value = instance.IAddProfileBsplineDLL(Properties, KnotArray, ControlPointCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` Curve IAddProfileBsplineDLL(     ref System.int Properties,    ref System.double KnotArray,    ref System.double ControlPointCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ IAddProfileBsplineDLL(  &   System.int% Properties, &   System.double% KnotArray, &   System.double% ControlPointCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Properties*

*KnotArray*

*ControlPointCoordArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::IAddProfileBsplineDLL.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)