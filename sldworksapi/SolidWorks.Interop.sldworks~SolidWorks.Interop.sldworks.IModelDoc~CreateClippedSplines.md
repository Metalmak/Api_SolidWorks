<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateClippedSplines.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateClippedSplines Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateClippedSplines Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ParamsIn*

*X1*

*Y1*

*X2*

*Y2*

Obsolete. Superseded by [IModelDoc2::CreateClippedSplines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateClippedSplines.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateClippedSplines( _    ByVal ParamsIn As System.Object, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim ParamsIn As System.Object Dim X1 As System.Double Dim Y1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim value As System.Object   value = instance.CreateClippedSplines(ParamsIn, X1, Y1, X2, Y2) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateClippedSplines(     System.object ParamsIn,    System.double X1,    System.double Y1,    System.double X2,    System.double Y2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateClippedSplines(  &   System.Object^ ParamsIn, &   System.double X1, &   System.double Y1, &   System.double X2, &   System.double Y2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ParamsIn*

*X1*

*Y1*

*X2*

*Y2*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateClippedSplines.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)