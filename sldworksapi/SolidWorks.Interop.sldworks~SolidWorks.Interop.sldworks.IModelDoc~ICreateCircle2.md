<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~ICreateCircle2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateCircle2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : ICreateCircle2 Method (IModelDoc) |

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

*Xp*

*Yp*

*Zp*

Obsolete. Superseded by [IModelDoc2::ICreateCircle2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ICreateCircle2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateCircle2( _    ByVal XC As System.Double, _    ByVal YC As System.Double, _    ByVal Zc As System.Double, _    ByVal Xp As System.Double, _    ByVal Yp As System.Double, _    ByVal Zp As System.Double _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim XC As System.Double Dim YC As System.Double Dim Zc As System.Double Dim Xp As System.Double Dim Yp As System.Double Dim Zp As System.Double Dim value As SketchSegment   value = instance.ICreateCircle2(XC, YC, Zc, Xp, Yp, Zp) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment ICreateCircle2(     System.double XC,    System.double YC,    System.double Zc,    System.double Xp,    System.double Yp,    System.double Zp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ ICreateCircle2(  &   System.double XC, &   System.double YC, &   System.double Zc, &   System.double Xp, &   System.double Yp, &   System.double Zp ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XC*

*YC*

*Zc*

*Xp*

*Yp*

*Zp*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::ICreateCircle2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)