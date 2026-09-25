<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateArcDB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateArcDB Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateArcDB Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X1*

*Y1*

*Z1*

*X2*

*Y2*

*Z2*

*X3*

*Y3*

*Z3*

*Dir*

Obsolete. Superseded by [IModelDoc2::CreateArc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateArc2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateArcDB( _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double, _    ByVal X3 As System.Double, _    ByVal Y3 As System.Double, _    ByVal Z3 As System.Double, _    ByVal Dir As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double Dim X3 As System.Double Dim Y3 As System.Double Dim Z3 As System.Double Dim Dir As System.Short Dim value As System.Boolean   value = instance.CreateArcDB(X1, Y1, Z1, X2, Y2, Z2, X3, Y3, Z3, Dir) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateArcDB(     System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2,    System.double X3,    System.double Y3,    System.double Z3,    System.short Dir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateArcDB(  &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2, &   System.double X3, &   System.double Y3, &   System.double Z3, &   System.short Dir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X1*

*Y1*

*Z1*

*X2*

*Y2*

*Z2*

*X3*

*Y3*

*Z3*

*Dir*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateArcDB.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)