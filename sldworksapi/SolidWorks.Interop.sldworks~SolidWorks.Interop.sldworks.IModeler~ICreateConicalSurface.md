<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateConicalSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateConicalSurface Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateConicalSurface Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*

*Direction*

*Radius*

*SemiAngle*

Obsolete. Superseded by [IModeler::ICreateConicalSurface2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICreateCylindricalSurface2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateConicalSurface( _    ByRef Center As System.Double, _    ByRef Direction As System.Double, _    ByVal Radius As System.Double, _    ByVal SemiAngle As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Center As System.Double Dim Direction As System.Double Dim Radius As System.Double Dim SemiAngle As System.Double Dim value As Surface   value = instance.ICreateConicalSurface(Center, Direction, Radius, SemiAngle) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateConicalSurface(     ref System.double Center,    ref System.double Direction,    System.double Radius,    System.double SemiAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateConicalSurface(  &   System.double% Center, &   System.double% Direction, &   System.double Radius, &   System.double SemiAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*

*Direction*

*Radius*

*SemiAngle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICreateConicalSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)