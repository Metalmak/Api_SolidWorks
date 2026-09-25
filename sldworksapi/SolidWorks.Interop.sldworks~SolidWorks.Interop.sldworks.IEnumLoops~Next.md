<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumLoops~Next.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Next Method (IEnumLoops) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumLoops Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumLoops.html) : Next Method (IEnumLoops) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Celt*

*Rgelt*

*PceltFetched*

Obsolete. Superseded by [IEnumLoops2::Next](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumLoops2~Next.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Next( _    ByVal Celt As System.Integer, _    ByRef Rgelt As Loop, _    ByRef PceltFetched As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumLoops Dim Celt As System.Integer Dim Rgelt As Loop Dim PceltFetched As System.Integer   instance.Next(Celt, Rgelt, PceltFetched) ``` | |

| C# |  |
| --- | --- |
| ``` void Next(     System.int Celt,    out Loop Rgelt,    out System.int PceltFetched ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Next(  &   System.int Celt, &   [Out] Loop^ Rgelt, &   [Out] System.int PceltFetched ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Celt*

*Rgelt*

*PceltFetched*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumLoops::Next.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumLoops Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumLoops.html)

[IEnumLoops Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumLoops_members.html)