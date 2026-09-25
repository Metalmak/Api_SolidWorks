<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~AddTrimmingLoop.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddTrimmingLoop Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : AddTrimmingLoop Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCrvs*

*VOrder*

*VDim*

*VPeriodic*

*VNumKnots*

*VNumCtrlPoints*

*VKnots*

*VCtrlPointDbls*

Obsolete. Superseded by [ISurface::AddTrimmingLoop2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~AddTrimmingLoop2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddTrimmingLoop( _    ByVal NCrvs As System.Integer, _    ByVal VOrder As System.Object, _    ByVal VDim As System.Object, _    ByVal VPeriodic As System.Object, _    ByVal VNumKnots As System.Object, _    ByVal VNumCtrlPoints As System.Object, _    ByVal VKnots As System.Object, _    ByVal VCtrlPointDbls As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim NCrvs As System.Integer Dim VOrder As System.Object Dim VDim As System.Object Dim VPeriodic As System.Object Dim VNumKnots As System.Object Dim VNumCtrlPoints As System.Object Dim VKnots As System.Object Dim VCtrlPointDbls As System.Object Dim value As System.Boolean   value = instance.AddTrimmingLoop(NCrvs, VOrder, VDim, VPeriodic, VNumKnots, VNumCtrlPoints, VKnots, VCtrlPointDbls) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddTrimmingLoop(     System.int NCrvs,    System.object VOrder,    System.object VDim,    System.object VPeriodic,    System.object VNumKnots,    System.object VNumCtrlPoints,    System.object VKnots,    System.object VCtrlPointDbls ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddTrimmingLoop(  &   System.int NCrvs, &   System.Object^ VOrder, &   System.Object^ VDim, &   System.Object^ VPeriodic, &   System.Object^ VNumKnots, &   System.Object^ VNumCtrlPoints, &   System.Object^ VKnots, &   System.Object^ VCtrlPointDbls ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NCrvs*

*VOrder*

*VDim*

*VPeriodic*

*VNumKnots*

*VNumCtrlPoints*

*VKnots*

*VCtrlPointDbls*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::AddTrimmingLoop.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)