<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumDisplayDimensions~Next.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Next Method (IEnumDisplayDimensions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumDisplayDimensions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumDisplayDimensions.html) : Next Method (IEnumDisplayDimensions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Celt*
:   Number of display dimensions for the display dimension enumeration

*Rgelt*
:   Pointer to an array of [display dimensions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html) in of size Celt

*PceltFetched*
:   Pointer to the number of display dimensions from the list; this value can be less than Celt if you ask for more display dimensions than exist, or it can be
    NULL if no more display dimensions exist

Gets the next display dimension in the display dimensions enumeration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Next( _    ByVal Celt As System.Integer, _    ByRef Rgelt As DisplayDimension, _    ByRef PceltFetched As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumDisplayDimensions Dim Celt As System.Integer Dim Rgelt As DisplayDimension Dim PceltFetched As System.Integer   instance.Next(Celt, Rgelt, PceltFetched) ``` | |

| C# |  |
| --- | --- |
| ``` void Next(     System.int Celt,    out DisplayDimension Rgelt,    out System.int PceltFetched ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Next(  &   System.int Celt, &   [Out] DisplayDimension^ Rgelt, &   [Out] System.int PceltFetched ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Celt*
:   Number of display dimensions for the display dimension enumeration

*Rgelt*
:   Pointer to an array of [display dimensions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html) in of size Celt

*PceltFetched*
:   Pointer to the number of display dimensions from the list; this value can be less than Celt if you ask for more display dimensions than exist, or it can be
    NULL if no more display dimensions exist

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumDisplayDimensions::Next.

# ![](dotnetimages/collapse.gif)Remarks

For use in in-process DLLs only.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumDisplayDimensions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumDisplayDimensions.html)

[IEnumDisplayDimensions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumDisplayDimensions_members.html)