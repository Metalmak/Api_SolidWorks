<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameSymbols.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFrameSymbols Method (IGtol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetFrameSymbols Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FrameNumber*

*GCS*

*TolDia1*

*TolMC1*

*TolDia2*

*TolMC2*

*DatumMC1*

*DatumMC2*

*DatumMC3*

Obsolete. Superseded by [IGtol::SetFrameSymbols2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~SetFrameSymbols2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFrameSymbols( _    ByVal FrameNumber As System.Short, _    ByVal GCS As System.Short, _    ByVal TolDia1 As System.Boolean, _    ByVal TolMC1 As System.Short, _    ByVal TolDia2 As System.Boolean, _    ByVal TolMC2 As System.Short, _    ByVal DatumMC1 As System.Short, _    ByVal DatumMC2 As System.Short, _    ByVal DatumMC3 As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim FrameNumber As System.Short Dim GCS As System.Short Dim TolDia1 As System.Boolean Dim TolMC1 As System.Short Dim TolDia2 As System.Boolean Dim TolMC2 As System.Short Dim DatumMC1 As System.Short Dim DatumMC2 As System.Short Dim DatumMC3 As System.Short   instance.SetFrameSymbols(FrameNumber, GCS, TolDia1, TolMC1, TolDia2, TolMC2, DatumMC1, DatumMC2, DatumMC3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFrameSymbols(     System.short FrameNumber,    System.short GCS,    System.bool TolDia1,    System.short TolMC1,    System.bool TolDia2,    System.short TolMC2,    System.short DatumMC1,    System.short DatumMC2,    System.short DatumMC3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFrameSymbols(  &   System.short FrameNumber, &   System.short GCS, &   System.bool TolDia1, &   System.short TolMC1, &   System.bool TolDia2, &   System.short TolMC2, &   System.short DatumMC1, &   System.short DatumMC2, &   System.short DatumMC3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FrameNumber*

*GCS*

*TolDia1*

*TolMC1*

*TolDia2*

*TolMC2*

*DatumMC1*

*DatumMC2*

*DatumMC3*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetFrameSymbols.

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)