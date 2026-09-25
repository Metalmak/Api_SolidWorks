<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateArc2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateArc2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateArc2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XC*

*YC*

*Zc*

*Xp1*

*Yp1*

*Zp1*

*Xp2*

*Yp2*

*Zp2*

*Direction*

Obsolete. Superseded by [IModelDoc2::CreateArc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateArc2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateArc2( _    ByVal XC As System.Double, _    ByVal YC As System.Double, _    ByVal Zc As System.Double, _    ByVal Xp1 As System.Double, _    ByVal Yp1 As System.Double, _    ByVal Zp1 As System.Double, _    ByVal Xp2 As System.Double, _    ByVal Yp2 As System.Double, _    ByVal Zp2 As System.Double, _    ByVal Direction As System.Short _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim XC As System.Double Dim YC As System.Double Dim Zc As System.Double Dim Xp1 As System.Double Dim Yp1 As System.Double Dim Zp1 As System.Double Dim Xp2 As System.Double Dim Yp2 As System.Double Dim Zp2 As System.Double Dim Direction As System.Short Dim value As System.Object   value = instance.CreateArc2(XC, YC, Zc, Xp1, Yp1, Zp1, Xp2, Yp2, Zp2, Direction) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateArc2(     System.double XC,    System.double YC,    System.double Zc,    System.double Xp1,    System.double Yp1,    System.double Zp1,    System.double Xp2,    System.double Yp2,    System.double Zp2,    System.short Direction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateArc2(  &   System.double XC, &   System.double YC, &   System.double Zc, &   System.double Xp1, &   System.double Yp1, &   System.double Zp1, &   System.double Xp2, &   System.double Yp2, &   System.double Zp2, &   System.short Direction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XC*

*YC*

*Zc*

*Xp1*

*Yp1*

*Zp1*

*Xp2*

*Yp2*

*Zp2*

*Direction*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateArc2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)