<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~ICreateBsplineSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBsplineSurfaceDLL Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : ICreateBsplineSurfaceDLL Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Properties*

*UKnotArray*

*VKnotArray*

*ControlPointCoordArray*

Obsolete. Superseded by [IBody2::ICreateBsplineSurfaceDLL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreateBsplineSurfaceDLL.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBsplineSurfaceDLL( _    ByRef Properties As System.Integer, _    ByRef UKnotArray As System.Double, _    ByRef VKnotArray As System.Double, _    ByRef ControlPointCoordArray As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Properties As System.Integer Dim UKnotArray As System.Double Dim VKnotArray As System.Double Dim ControlPointCoordArray As System.Double Dim value As Surface   value = instance.ICreateBsplineSurfaceDLL(Properties, UKnotArray, VKnotArray, ControlPointCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateBsplineSurfaceDLL(     ref System.int Properties,    ref System.double UKnotArray,    ref System.double VKnotArray,    ref System.double ControlPointCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateBsplineSurfaceDLL(  &   System.int% Properties, &   System.double% UKnotArray, &   System.double% VKnotArray, &   System.double% ControlPointCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Properties*

*UKnotArray*

*VKnotArray*

*ControlPointCoordArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::ICreateBsplineSurfaceDLL.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)