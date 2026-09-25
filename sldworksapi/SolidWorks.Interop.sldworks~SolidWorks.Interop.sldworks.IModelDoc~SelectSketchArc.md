<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SelectSketchArc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SelectSketchArc Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SelectSketchArc Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X0*

*Y0*

*Inc0*

*X1*

*Y1*

*Inc1*

*XC*

*YC*

*IncC*

*RotDir*

Obsolete. Superseded by [IModelDoc2::SelectSketchArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SelectSketchArc.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SelectSketchArc( _    ByVal X0 As System.Double, _    ByVal Y0 As System.Double, _    ByVal Inc0 As System.Integer, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Inc1 As System.Integer, _    ByVal XC As System.Double, _    ByVal YC As System.Double, _    ByVal IncC As System.Integer, _    ByVal RotDir As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim X0 As System.Double Dim Y0 As System.Double Dim Inc0 As System.Integer Dim X1 As System.Double Dim Y1 As System.Double Dim Inc1 As System.Integer Dim XC As System.Double Dim YC As System.Double Dim IncC As System.Integer Dim RotDir As System.Integer   instance.SelectSketchArc(X0, Y0, Inc0, X1, Y1, Inc1, XC, YC, IncC, RotDir) ``` | |

| C# |  |
| --- | --- |
| ``` void SelectSketchArc(     System.double X0,    System.double Y0,    System.int Inc0,    System.double X1,    System.double Y1,    System.int Inc1,    System.double XC,    System.double YC,    System.int IncC,    System.int RotDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SelectSketchArc(  &   System.double X0, &   System.double Y0, &   System.int Inc0, &   System.double X1, &   System.double Y1, &   System.int Inc1, &   System.double XC, &   System.double YC, &   System.int IncC, &   System.int RotDir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X0*

*Y0*

*Inc0*

*X1*

*Y1*

*Inc1*

*XC*

*YC*

*IncC*

*RotDir*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SelectSketchArc.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)