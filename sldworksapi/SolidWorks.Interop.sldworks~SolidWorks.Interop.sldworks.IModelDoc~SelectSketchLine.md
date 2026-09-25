<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SelectSketchLine.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SelectSketchLine Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SelectSketchLine Method (IModelDoc) |

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

Obsolete. Superseded by [IModelDoc2::SelectSketchLine](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SelectSketchLine.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SelectSketchLine( _    ByVal X0 As System.Double, _    ByVal Y0 As System.Double, _    ByVal Inc0 As System.Integer, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Inc1 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim X0 As System.Double Dim Y0 As System.Double Dim Inc0 As System.Integer Dim X1 As System.Double Dim Y1 As System.Double Dim Inc1 As System.Integer   instance.SelectSketchLine(X0, Y0, Inc0, X1, Y1, Inc1) ``` | |

| C# |  |
| --- | --- |
| ``` void SelectSketchLine(     System.double X0,    System.double Y0,    System.int Inc0,    System.double X1,    System.double Y1,    System.int Inc1 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SelectSketchLine(  &   System.double X0, &   System.double Y0, &   System.int Inc0, &   System.double X1, &   System.double Y1, &   System.int Inc1 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X0*

*Y0*

*Inc0*

*X1*

*Y1*

*Inc1*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SelectSketchLine.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)