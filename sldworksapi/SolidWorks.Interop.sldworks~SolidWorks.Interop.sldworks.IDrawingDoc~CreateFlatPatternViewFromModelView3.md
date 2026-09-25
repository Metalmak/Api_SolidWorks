<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateFlatPatternViewFromModelView3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFlatPatternViewFromModelView3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateFlatPatternViewFromModelView3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelName*
:   Name of model

*ConfigName*
:   Name of configuration

*LocX*
:   X coordinate

*LocY*
:   Y coordinate

*LocZ*
:   Z coordinate

*HideBendLines*
:   True hides bend lines, false does not

*FlipView*
:   True flips the view, false does not

Creates a flat-pattern view from a model view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFlatPatternViewFromModelView3( _    ByVal ModelName As System.String, _    ByVal ConfigName As System.String, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double, _    ByVal HideBendLines As System.Boolean, _    ByVal FlipView As System.Boolean _ ) As View ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim ModelName As System.String Dim ConfigName As System.String Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim HideBendLines As System.Boolean Dim FlipView As System.Boolean Dim value As View   value = instance.CreateFlatPatternViewFromModelView3(ModelName, ConfigName, LocX, LocY, LocZ, HideBendLines, FlipView) ``` | |

| C# |  |
| --- | --- |
| ``` View CreateFlatPatternViewFromModelView3(     System.string ModelName,    System.string ConfigName,    System.double LocX,    System.double LocY,    System.double LocZ,    System.bool HideBendLines,    System.bool FlipView ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` View^ CreateFlatPatternViewFromModelView3(  &   System.String^ ModelName, &   System.String^ ConfigName, &   System.double LocX, &   System.double LocY, &   System.double LocZ, &   System.bool HideBendLines, &   System.bool FlipView ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelName*
:   Name of model

*ConfigName*
:   Name of configuration

*LocX*
:   X coordinate

*LocY*
:   Y coordinate

*LocZ*
:   Z coordinate

*HideBendLines*
:   True hides bend lines, false does not

*FlipView*
:   True flips the view, false does not

#### Return Value

Flat-pattern [view](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateFlatPatternViewFromModelView3.

# ![](dotnetimages/collapse.gif)Example

[Create and Flip Flat-Pattern View of Sheet Metal Part (VBA)](Create_and_Flip_Flat-Pattern_View_of_Sheet_Metal_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IView::FlipView Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~FlipView.html)

[IView::IsFlatPatternView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsFlatPatternView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP5, Revision Number 15.5