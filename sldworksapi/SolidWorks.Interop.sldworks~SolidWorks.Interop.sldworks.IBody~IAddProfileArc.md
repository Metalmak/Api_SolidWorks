<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~IAddProfileArc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddProfileArc Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : IAddProfileArc Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*

*Axis*

*Radius*

*StartPoint*

*EndPoint*

Obsolete. Superseded by [IBody2::IAddProfileArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IAddProfileArc.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddProfileArc( _    ByVal Center As System.Object, _    ByVal Axis As System.Object, _    ByVal Radius As System.Double, _    ByVal StartPoint As System.Object, _    ByVal EndPoint As System.Object _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Center As System.Object Dim Axis As System.Object Dim Radius As System.Double Dim StartPoint As System.Object Dim EndPoint As System.Object Dim value As Curve   value = instance.IAddProfileArc(Center, Axis, Radius, StartPoint, EndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` Curve IAddProfileArc(     System.object Center,    System.object Axis,    System.double Radius,    System.object StartPoint,    System.object EndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ IAddProfileArc(  &   System.Object^ Center, &   System.Object^ Axis, &   System.double Radius, &   System.Object^ StartPoint, &   System.Object^ EndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*

*Axis*

*Radius*

*StartPoint*

*EndPoint*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::IAddProfileArc.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)