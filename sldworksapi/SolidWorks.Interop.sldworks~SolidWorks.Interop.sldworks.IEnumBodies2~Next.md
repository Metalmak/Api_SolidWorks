<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumBodies2~Next.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Next Method (IEnumBodies2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumBodies2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumBodies2.html) : Next Method (IEnumBodies2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Celt*
:   Number of bodies for the bodies enumeration

*Rgelt*
:   Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) of size Celt

*PceltFetched*
:   Pointer to the number of bodies returned from the list; this value can be less than Celt if you request more bodies than exist, or it can be NULL if no more bodies exist

Gets the next body in the bodies enumeration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Next( _    ByVal Celt As System.Integer, _    ByRef Rgelt As Body2, _    ByRef PceltFetched As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumBodies2 Dim Celt As System.Integer Dim Rgelt As Body2 Dim PceltFetched As System.Integer   instance.Next(Celt, Rgelt, PceltFetched) ``` | |

| C# |  |
| --- | --- |
| ``` void Next(     System.int Celt,    out Body2 Rgelt,    out System.int PceltFetched ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Next(  &   System.int Celt, &   [Out] Body2^ Rgelt, &   [Out] System.int PceltFetched ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Celt*
:   Number of bodies for the bodies enumeration

*Rgelt*
:   Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) of size Celt

*PceltFetched*
:   Pointer to the number of bodies returned from the list; this value can be less than Celt if you request more bodies than exist, or it can be NULL if no more bodies exist

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumBodies2::Next.

# ![](dotnetimages/collapse.gif)Example

[Enumerate Bodies (C++)](Enumerate_Bodies_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

For use in in-process DLLs only.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumBodies2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumBodies2.html)

[IEnumBodies2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumBodies2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0