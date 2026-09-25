<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~GetExtremePoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetExtremePoint Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : GetExtremePoint Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*

*Y*

*Z*

*Outx*

*Outy*

*Outz*

Obsolete. Superseded by [IBody2::GetExtremePoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetExtremePoint.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetExtremePoint( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByRef Outx As System.Double, _    ByRef Outy As System.Double, _    ByRef Outz As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim Outx As System.Double Dim Outy As System.Double Dim Outz As System.Double Dim value As System.Boolean   value = instance.GetExtremePoint(X, Y, Z, Outx, Outy, Outz) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetExtremePoint(     System.double X,    System.double Y,    System.double Z,    out System.double Outx,    out System.double Outy,    out System.double Outz ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetExtremePoint(  &   System.double X, &   System.double Y, &   System.double Z, &   [Out] System.double Outx, &   [Out] System.double Outy, &   [Out] System.double Outz ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*

*Y*

*Z*

*Outx*

*Outy*

*Outz*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::GetExtremePoint.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)