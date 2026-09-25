<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IGetBSurfParamsSize2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetBSurfParamsSize2 Method (ISurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IGetBSurfParamsSize2 Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WantCubic*

*WantNonRational*

*Range*

Obsolete. Superseded by [ISurface::IGetBSurfParamsSize3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IGetBSurfParamsSize3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetBSurfParamsSize2( _    ByVal WantCubic As System.Boolean, _    ByVal WantNonRational As System.Boolean, _    ByRef Range As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim WantCubic As System.Boolean Dim WantNonRational As System.Boolean Dim Range As System.Double Dim value As System.Integer   value = instance.IGetBSurfParamsSize2(WantCubic, WantNonRational, Range) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetBSurfParamsSize2(     System.bool WantCubic,    System.bool WantNonRational,    ref System.double Range ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetBSurfParamsSize2(  &   System.bool WantCubic, &   System.bool WantNonRational, &   System.double% Range ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WantCubic*

*WantNonRational*

*Range*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IGetBSurfParamsSize2.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)