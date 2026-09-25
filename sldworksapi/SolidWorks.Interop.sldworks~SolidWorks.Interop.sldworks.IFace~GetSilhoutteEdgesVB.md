<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace~GetSilhoutteEdgesVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSilhoutteEdgesVB Method (IFace) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html) : GetSilhoutteEdgesVB Method (IFace) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Xroot*

*Yroot*

*Zroot*

*Xnormal*

*Ynormal*

*Znormal*

Obsolete. Superseded by [IFace2::GetSilhoutteEdgesVB](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetSilhoutteEdgesVB.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSilhoutteEdgesVB( _    ByVal Xroot As System.Double, _    ByVal Yroot As System.Double, _    ByVal Zroot As System.Double, _    ByVal Xnormal As System.Double, _    ByVal Ynormal As System.Double, _    ByVal Znormal As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace Dim Xroot As System.Double Dim Yroot As System.Double Dim Zroot As System.Double Dim Xnormal As System.Double Dim Ynormal As System.Double Dim Znormal As System.Double Dim value As System.Object   value = instance.GetSilhoutteEdgesVB(Xroot, Yroot, Zroot, Xnormal, Ynormal, Znormal) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSilhoutteEdgesVB(     System.double Xroot,    System.double Yroot,    System.double Zroot,    System.double Xnormal,    System.double Ynormal,    System.double Znormal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSilhoutteEdgesVB(  &   System.double Xroot, &   System.double Yroot, &   System.double Zroot, &   System.double Xnormal, &   System.double Ynormal, &   System.double Znormal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Xroot*

*Yroot*

*Zroot*

*Xnormal*

*Ynormal*

*Znormal*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face::GetSilhoutteEdgesVB.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html)

[IFace Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace_members.html)