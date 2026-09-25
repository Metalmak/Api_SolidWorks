<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateText Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateText Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TextString*

*TextX*

*TextY*

*TextZ*

*TextHeight*

*TextAngle*

Obsolete. Superseded by [IDrawingDoc::CreateText2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateText2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateText( _    ByVal TextString As System.String, _    ByVal TextX As System.Double, _    ByVal TextY As System.Double, _    ByVal TextZ As System.Double, _    ByVal TextHeight As System.Double, _    ByVal TextAngle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim TextString As System.String Dim TextX As System.Double Dim TextY As System.Double Dim TextZ As System.Double Dim TextHeight As System.Double Dim TextAngle As System.Double Dim value As System.Boolean   value = instance.CreateText(TextString, TextX, TextY, TextZ, TextHeight, TextAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateText(     System.string TextString,    System.double TextX,    System.double TextY,    System.double TextZ,    System.double TextHeight,    System.double TextAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateText(  &   System.String^ TextString, &   System.double TextX, &   System.double TextY, &   System.double TextZ, &   System.double TextHeight, &   System.double TextAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TextString*

*TextX*

*TextY*

*TextZ*

*TextHeight*

*TextAngle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateText.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)