<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~ICreateRevolutionSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateRevolutionSurfaceDLL Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : ICreateRevolutionSurfaceDLL Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ProfileCurve*

*AxisPoint*

*AxisDirection*

*ProfileEndPtParams*

Obsolete. Superseded by [IBody2::ICreateRevolutionSurfaceDLL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreateRevolutionSurfaceDLL.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateRevolutionSurfaceDLL( _    ByVal ProfileCurve As Curve, _    ByRef AxisPoint As System.Double, _    ByRef AxisDirection As System.Double, _    ByRef ProfileEndPtParams As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim ProfileCurve As Curve Dim AxisPoint As System.Double Dim AxisDirection As System.Double Dim ProfileEndPtParams As System.Double Dim value As Surface   value = instance.ICreateRevolutionSurfaceDLL(ProfileCurve, AxisPoint, AxisDirection, ProfileEndPtParams) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateRevolutionSurfaceDLL(     Curve ProfileCurve,    ref System.double AxisPoint,    ref System.double AxisDirection,    ref System.double ProfileEndPtParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateRevolutionSurfaceDLL(  &   Curve^ ProfileCurve, &   System.double% AxisPoint, &   System.double% AxisDirection, &   System.double% ProfileEndPtParams ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProfileCurve*

*AxisPoint*

*AxisDirection*

*ProfileEndPtParams*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::ICreateRevolutionSurfaceDLL.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)