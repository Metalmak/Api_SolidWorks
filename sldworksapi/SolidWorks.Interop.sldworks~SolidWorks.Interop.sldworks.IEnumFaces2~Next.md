<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces2~Next.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Next Method (IEnumFaces2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumFaces2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces2.html) : Next Method (IEnumFaces2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Celt*
:   Number of faces for the faces enumeration

*Rgelt*
:   Pointer to an array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of size Celt

*PceltFetched*
:   Pointer to the number of faces returned from the list; this value can be less than Celt if you asked for more faces than exist, or it can be NULL if no more faces exist

Gets the next face in the faces enumeration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Next( _    ByVal Celt As System.Integer, _    ByRef Rgelt As Face2, _    ByRef PceltFetched As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumFaces2 Dim Celt As System.Integer Dim Rgelt As Face2 Dim PceltFetched As System.Integer   instance.Next(Celt, Rgelt, PceltFetched) ``` | |

| C# |  |
| --- | --- |
| ``` void Next(     System.int Celt,    out Face2 Rgelt,    out System.int PceltFetched ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Next(  &   System.int Celt, &   [Out] Face2^ Rgelt, &   [Out] System.int PceltFetched ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Celt*
:   Number of faces for the faces enumeration

*Rgelt*
:   Pointer to an array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of size Celt

*PceltFetched*
:   Pointer to the number of faces returned from the list; this value can be less than Celt if you asked for more faces than exist, or it can be NULL if no more faces exist

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumFaces2::Next.

# ![](dotnetimages/collapse.gif)Remarks

For use in in-process DLLs only.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumFaces2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces2.html)

[IEnumFaces2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumFaces2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0