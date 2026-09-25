<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDrawViewFromModelView2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateDrawViewFromModelView2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateDrawViewFromModelView2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelName*

*ViewName*

*LocX*

*LocY*

*LocZ*

Obsolete. Superseded by [IDrawingDoc::CreateDrawViewFromModelView3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateDrawViewFromModelView3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateDrawViewFromModelView2( _    ByVal ModelName As System.String, _    ByVal ViewName As System.String, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double _ ) As View ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim ModelName As System.String Dim ViewName As System.String Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim value As View   value = instance.CreateDrawViewFromModelView2(ModelName, ViewName, LocX, LocY, LocZ) ``` | |

| C# |  |
| --- | --- |
| ``` View CreateDrawViewFromModelView2(     System.string ModelName,    System.string ViewName,    System.double LocX,    System.double LocY,    System.double LocZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` View^ CreateDrawViewFromModelView2(  &   System.String^ ModelName, &   System.String^ ViewName, &   System.double LocX, &   System.double LocY, &   System.double LocZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelName*

*ViewName*

*LocX*

*LocY*

*LocZ*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateDrawViewFromModelView2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)