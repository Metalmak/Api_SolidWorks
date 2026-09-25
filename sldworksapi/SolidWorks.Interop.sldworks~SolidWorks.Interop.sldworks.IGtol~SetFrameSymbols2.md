<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameSymbols2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFrameSymbols2 Method (IGtol) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetFrameSymbols2 Method (IGtol) |

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

*GCS*
:   Geometric tolerance symbol (see **Remarks**)

*TolDia1*
:   Diameter symbol exists for tolerance 1 (True or false)

*TolMC1*
:   Material condition symbol for tolerance 1 (see **Remarks**)

*TolDia2*
:   Diameter symbol exists for tolerance 2 (True or false)

*TolMC2*
:   Material condition symbol for tolerance 2 (see **Remarks**)

*DatumMC1*
:   Material condition symbols for primary datum (see **Remarks**)

*DatumMC2*
:   Material condition symbols for secondary datum (see **Remarks**)

*DatumMC3*
:   Material condition symbols for tertiary datum (see **Remarks**)

Sets the symbols for the specified frame.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFrameSymbols2( _    ByVal FrameNumber As System.Short, _    ByVal GCS As System.String, _    ByVal TolDia1 As System.Boolean, _    ByVal TolMC1 As System.String, _    ByVal TolDia2 As System.Boolean, _    ByVal TolMC2 As System.String, _    ByVal DatumMC1 As System.String, _    ByVal DatumMC2 As System.String, _    ByVal DatumMC3 As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim FrameNumber As System.Short Dim GCS As System.String Dim TolDia1 As System.Boolean Dim TolMC1 As System.String Dim TolDia2 As System.Boolean Dim TolMC2 As System.String Dim DatumMC1 As System.String Dim DatumMC2 As System.String Dim DatumMC3 As System.String   instance.SetFrameSymbols2(FrameNumber, GCS, TolDia1, TolMC1, TolDia2, TolMC2, DatumMC1, DatumMC2, DatumMC3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFrameSymbols2(     System.short FrameNumber,    System.string GCS,    System.bool TolDia1,    System.string TolMC1,    System.bool TolDia2,    System.string TolMC2,    System.string DatumMC1,    System.string DatumMC2,    System.string DatumMC3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFrameSymbols2(  &   System.short FrameNumber, &   System.String^ GCS, &   System.bool TolDia1, &   System.String^ TolMC1, &   System.bool TolDia2, &   System.String^ TolMC2, &   System.String^ DatumMC1, &   System.String^ DatumMC2, &   System.String^ DatumMC3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FrameNumber*
:   Feature control frame 1 for first

*GCS*
:   Geometric tolerance symbol (see **Remarks**)

*TolDia1*
:   Diameter symbol exists for tolerance 1 (True or false)

*TolMC1*
:   Material condition symbol for tolerance 1 (see **Remarks**)

*TolDia2*
:   Diameter symbol exists for tolerance 2 (True or false)

*TolMC2*
:   Material condition symbol for tolerance 2 (see **Remarks**)

*DatumMC1*
:   Material condition symbols for primary datum (see **Remarks**)

*DatumMC2*
:   Material condition symbols for secondary datum (see **Remarks**)

*DatumMC3*
:   Material condition symbols for tertiary datum (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetFrameSymbols2.

# ![](dotnetimages/collapse.gif)Example

[Insert GTol (C#)](Insert_GTol_Example_CSharp.htm)

[Insert GTol (VB.NET)](Insert_GTol_Example_VBNET.htm)

[Insert GTol (VBA)](Insert_GTol_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

GTol symbols are defined in **C:\ProgramData\SolidWorks\SolidWorks** **20***nn***\lang\english\**gtol.sym. Reference this file to specify GCS, TolMC1, TolMC2, DatumMC1, DatumMC2, and DatumMC3 in <*LibraryName-SymbolName*> format.

Examples:

* GCS = "<IGTOL-POSI>" (Position symbol in the ISO Geometric Tolerancing Symbols library)* TolMC1 = "<MOD-LMC>" (Least Material Condition symbol in the Modifying Symbols library)

After calling this method, call [IGtol::SetFrameValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetFrameValues2.html) to specify tolerance and datum values.

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::GetFrameCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameCount.html)

[IGtol::GetFrameDiameterSymbols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameDiameterSymbols.html)

[IGtol::GetFrameSymbols2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameSymbols2.html)

[IGtol::GetFrameValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetFrameValues.html)

[IGtol::IGetFrameDiameterSymbols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetFrameDiameterSymbols.html)

[IGtol::IGetFrameSymbols2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetFrameSymbols2.html)

[IGtol::IGetFrameValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetFrameValues.html)