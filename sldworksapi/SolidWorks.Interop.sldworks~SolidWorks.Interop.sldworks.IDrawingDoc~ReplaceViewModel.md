<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ReplaceViewModel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceViewModel Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ReplaceViewModel Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NewModelPathName*
:   Full path and filename of the replacement model

*Views*
:   Array of [IView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)s in which to replace the model

*Instances*
:   Array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)s that are specific instances of the model to replace in the drawing

Replaces the specified instances of a model in the specified drawing views.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceViewModel( _    ByVal NewModelPathName As System.String, _    ByVal Views As System.Object, _    ByVal Instances As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim NewModelPathName As System.String Dim Views As System.Object Dim Instances As System.Object Dim value As System.Boolean   value = instance.ReplaceViewModel(NewModelPathName, Views, Instances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceViewModel(     System.string NewModelPathName,    System.object Views,    System.object Instances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceViewModel(  &   System.String^ NewModelPathName, &   System.Object^ Views, &   System.Object^ Instances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NewModelPathName*
:   Full path and filename of the replacement model

*Views*
:   Array of [IView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)s in which to replace the model

*Instances*
:   Array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)s that are specific instances of the model to replace in the drawing

#### Return Value

True if the model is replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ReplaceViewModel.

# ![](dotnetimages/collapse.gif)Example

[Replace View Model (C#)](Replace_View_Model_Example_CSharp.htm)

[Replace View Model (VB.NET)](Replace_View_Model_Example_VBNET.htm)

[Replace View Model (VBA)](Replace_View_Model_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method corresponds to **Tools > Replace Model**.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::InsertModelInPredefinedView Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertModelInPredefinedView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0