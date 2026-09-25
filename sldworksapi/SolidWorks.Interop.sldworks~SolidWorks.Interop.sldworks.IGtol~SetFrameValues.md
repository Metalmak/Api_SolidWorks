<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFrameValues Method (IGtol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetFrameValues Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FrameNumber*
:   Feature control frame 1 for first

*Tol1*
:   Tolerance 1 value

*Tol2*
:   Tolerance 2 value

*Datum1*
:   Datum reference 1 (primary datum)

*Datum2*
:   Datum reference 2 (secondary datum)

*Datum3*
:   Datum reference 3 (tertiary datum)

Obsolete. Superseded by [IGtol::SetFrameValues2.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameValues2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFrameValues( _    ByVal FrameNumber As System.Short, _    ByVal Tol1 As System.String, _    ByVal Tol2 As System.String, _    ByVal Datum1 As System.String, _    ByVal Datum2 As System.String, _    ByVal Datum3 As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim FrameNumber As System.Short Dim Tol1 As System.String Dim Tol2 As System.String Dim Datum1 As System.String Dim Datum2 As System.String Dim Datum3 As System.String   instance.SetFrameValues(FrameNumber, Tol1, Tol2, Datum1, Datum2, Datum3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFrameValues(     System.short FrameNumber,    System.string Tol1,    System.string Tol2,    System.string Datum1,    System.string Datum2,    System.string Datum3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFrameValues(  &   System.short FrameNumber, &   System.String^ Tol1, &   System.String^ Tol2, &   System.String^ Datum1, &   System.String^ Datum2, &   System.String^ Datum3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FrameNumber*
:   Feature control frame 1 for first

*Tol1*
:   Tolerance 1 value

*Tol2*
:   Tolerance 2 value

*Datum1*
:   Datum reference 1 (primary datum)

*Datum2*
:   Datum reference 2 (secondary datum)

*Datum3*
:   Datum reference 3 (tertiary datum)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetFrameValues.

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::GetFrameCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameCount.html)

[IGtol::GetFrameDiameterSymbols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameDiameterSymbols.html)

[IGtol::GetFrameSymbols2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameSymbols2.html)

[IGtol::GetFrameValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameValues.html)

[IGtol::IGetFrameSymbols2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetFrameSymbols2.html)

[IGtol::IGetFrameValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetFrameValues.html)

[IGtol::SetFrameSymbols2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameSymbols2.html)