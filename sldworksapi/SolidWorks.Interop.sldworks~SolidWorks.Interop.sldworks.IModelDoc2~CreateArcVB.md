<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateArcVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateArcVB Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateArcVB Method (IModelDoc2) |

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

*P3x*

*P3y*

*P3z*

*Dir*

Obsolete. Superseded by [IModelDoc2::CreateArc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateArc2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub CreateArcVB( _    ByVal P1x As System.Double, _    ByVal P1y As System.Double, _    ByVal P1z As System.Double, _    ByVal P2x As System.Double, _    ByVal P2y As System.Double, _    ByVal P2z As System.Double, _    ByVal P3x As System.Double, _    ByVal P3y As System.Double, _    ByVal P3z As System.Double, _    ByVal Dir As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim P1x As System.Double Dim P1y As System.Double Dim P1z As System.Double Dim P2x As System.Double Dim P2y As System.Double Dim P2z As System.Double Dim P3x As System.Double Dim P3y As System.Double Dim P3z As System.Double Dim Dir As System.Short   instance.CreateArcVB(P1x, P1y, P1z, P2x, P2y, P2z, P3x, P3y, P3z, Dir) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateArcVB(     System.double P1x,    System.double P1y,    System.double P1z,    System.double P2x,    System.double P2y,    System.double P2z,    System.double P3x,    System.double P3y,    System.double P3z,    System.short Dir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateArcVB(  &   System.double P1x, &   System.double P1y, &   System.double P1z, &   System.double P2x, &   System.double P2y, &   System.double P2z, &   System.double P3x, &   System.double P3y, &   System.double P3z, &   System.short Dir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*P1x*

*P1y*

*P1z*

*P2x*

*P2y*

*P2z*

*P3x*

*P3y*

*P3z*

*Dir*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateArcVB.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)