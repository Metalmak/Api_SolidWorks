<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface~IGetFirstFace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetFirstFace Method (IMidSurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMidSurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface.html) : IGetFirstFace Method (IMidSurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FromFace1Disp*

*FromFace2Disp*

*Thickness*

Obsolete. Superseded by [IMidSurface2::IGetFirstFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMidSurface2~IGetFirstFace.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetFirstFace( _    ByRef FromFace1Disp As Face, _    ByRef FromFace2Disp As Face, _    ByRef Thickness As System.Double _ ) As Face ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMidSurface Dim FromFace1Disp As Face Dim FromFace2Disp As Face Dim Thickness As System.Double Dim value As Face   value = instance.IGetFirstFace(FromFace1Disp, FromFace2Disp, Thickness) ``` | |

| C# |  |
| --- | --- |
| ``` Face IGetFirstFace(     out Face FromFace1Disp,    out Face FromFace2Disp,    out System.double Thickness ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Face^ IGetFirstFace(  &   [Out] Face^ FromFace1Disp, &   [Out] Face^ FromFace2Disp, &   [Out] System.double Thickness ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromFace1Disp*

*FromFace2Disp*

*Thickness*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MidSurface::IGetFirstFace.

# ![](dotnetimages/collapse.gif)See Also

####

[IMidSurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface.html)

[IMidSurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface_members.html)