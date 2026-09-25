<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertTableAnnotation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertTableAnnotation Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertTableAnnotation Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*

*Y*

*AnchorType*

*Rows*

*Columns*

Obsolete. Superseded by [IDrawingDoc::InsertTableAnnotation2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertTableAnnotation2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertTableAnnotation( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal Rows As System.Integer, _    ByVal Columns As System.Integer _ ) As TableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim Rows As System.Integer Dim Columns As System.Integer Dim value As TableAnnotation   value = instance.InsertTableAnnotation(X, Y, AnchorType, Rows, Columns) ``` | |

| C# |  |
| --- | --- |
| ``` TableAnnotation InsertTableAnnotation(     System.double X,    System.double Y,    System.int AnchorType,    System.int Rows,    System.int Columns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TableAnnotation^ InsertTableAnnotation(  &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.int Rows, &   System.int Columns ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*

*Y*

*AnchorType*

*Rows*

*Columns*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertTableAnnotation.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)