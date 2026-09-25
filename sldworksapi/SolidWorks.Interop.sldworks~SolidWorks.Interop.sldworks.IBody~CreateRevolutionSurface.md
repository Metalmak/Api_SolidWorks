<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~CreateRevolutionSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateRevolutionSurface Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : CreateRevolutionSurface Method (IBody) |

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

Obsolete. Superseded by [IBody2::CreateRevolutionSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateRevolutionSurface.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateRevolutionSurface( _    ByVal ProfileCurve As System.Object, _    ByVal AxisPoint As System.Object, _    ByVal AxisDirection As System.Object, _    ByVal ProfileEndPtParams As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim ProfileCurve As System.Object Dim AxisPoint As System.Object Dim AxisDirection As System.Object Dim ProfileEndPtParams As System.Object Dim value As System.Object   value = instance.CreateRevolutionSurface(ProfileCurve, AxisPoint, AxisDirection, ProfileEndPtParams) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateRevolutionSurface(     System.object ProfileCurve,    System.object AxisPoint,    System.object AxisDirection,    System.object ProfileEndPtParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateRevolutionSurface(  &   System.Object^ ProfileCurve, &   System.Object^ AxisPoint, &   System.Object^ AxisDirection, &   System.Object^ ProfileEndPtParams ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProfileCurve*

*AxisPoint*

*AxisDirection*

*ProfileEndPtParams*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::CreateRevolutionSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)