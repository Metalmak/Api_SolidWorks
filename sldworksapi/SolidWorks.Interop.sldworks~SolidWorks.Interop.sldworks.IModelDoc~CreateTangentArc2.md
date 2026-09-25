<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateTangentArc2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateTangentArc2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateTangentArc2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*P1x*

*P1y*

*P1z*

*P2x*

*P2y*

*P2z*

*ArcTypeIn*

Obsolete. Superseded by [IModelDoc2::CreateTangentArc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateTangentArc2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateTangentArc2( _    ByVal P1x As System.Double, _    ByVal P1y As System.Double, _    ByVal P1z As System.Double, _    ByVal P2x As System.Double, _    ByVal P2y As System.Double, _    ByVal P2z As System.Double, _    ByVal ArcTypeIn As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim P1x As System.Double Dim P1y As System.Double Dim P1z As System.Double Dim P2x As System.Double Dim P2y As System.Double Dim P2z As System.Double Dim ArcTypeIn As System.Integer Dim value As System.Boolean   value = instance.CreateTangentArc2(P1x, P1y, P1z, P2x, P2y, P2z, ArcTypeIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateTangentArc2(     System.double P1x,    System.double P1y,    System.double P1z,    System.double P2x,    System.double P2y,    System.double P2z,    System.int ArcTypeIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateTangentArc2(  &   System.double P1x, &   System.double P1y, &   System.double P1z, &   System.double P2x, &   System.double P2y, &   System.double P2z, &   System.int ArcTypeIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*P1x*

*P1y*

*P1z*

*P2x*

*P2y*

*P2z*

*ArcTypeIn*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateTangentArc2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)