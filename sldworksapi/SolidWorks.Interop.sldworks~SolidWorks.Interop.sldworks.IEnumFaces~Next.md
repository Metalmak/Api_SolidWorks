<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces~Next.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Next Method (IEnumFaces) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumFaces Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces.html) : Next Method (IEnumFaces) |

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

Obsolete. Superseded by [IEnumFaces2::Next](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumFaces2~Next.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Next( _    ByVal Celt As System.Integer, _    ByRef Rgelt As Face, _    ByRef PceltFetched As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumFaces Dim Celt As System.Integer Dim Rgelt As Face Dim PceltFetched As System.Integer   instance.Next(Celt, Rgelt, PceltFetched) ``` | |

| C# |  |
| --- | --- |
| ``` void Next(     System.int Celt,    out Face Rgelt,    out System.int PceltFetched ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Next(  &   System.int Celt, &   [Out] Face^ Rgelt, &   [Out] System.int PceltFetched ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Celt*

*Rgelt*

*PceltFetched*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumFaces::Next.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumFaces Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces.html)

[IEnumFaces Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces_members.html)