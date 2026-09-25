<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~HideShowDrawingViews.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| HideShowDrawingViews Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : HideShowDrawingViews Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets whether to hide or show hidden drawing views.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub HideShowDrawingViews() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc   instance.HideShowDrawingViews() ``` | |

| C# |  |
| --- | --- |
| ``` void HideShowDrawingViews() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void HideShowDrawingViews(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::HideShowDrawingViews.

# ![](dotnetimages/collapse.gif)Example

[Display Hidden Lines in Drawing (VBA)](Display_Hidden_Lines_in_Drawing_Example_VB.htm)

[Display Hidden Lines in Drawing (VB.NET)](Display_Hidden_Lines_in_Drawing_Example_VBNET.htm)

[Display Hidden Lines in Drawing (C#)](Display_Hidden_Lines_in_Drawing_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this setting is enabled, then SOLIDWORKS shows drawing views that were hidden using [IDrawingDoc::SuppressView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~SuppressView.html) with an **X**.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::ActivateView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ActivateView.html)

[IDrawingDoc::SuppressView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SuppressView.html)

[IDrawingDoc::UnsuppressView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~UnsuppressView.html)

[IDrawingDoc::ViewDisplayHidden Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewDisplayHidden.html)

[IDrawingDoc::ViewDisplayHiddengreyed Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewDisplayHiddengreyed.html)

[IDrawingDoc::ViewDisplayShaded Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewDisplayShaded.html)

[IDrawingDoc::ViewDisplayWireframe Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewDisplayWireframe.html)

[IDrawingDoc::ViewFullPage Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewFullPage.html)

[IDrawingDoc::ViewHlrQuality Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ViewHlrQuality.html)

[IDrawingDoc::ActiveDrawingView Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ActiveDrawingView.html)

[IDrawingDoc::AutomaticViewUpdate Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AutomaticViewUpdate.html)

[IDrawingDoc::HiddenViewsVisible Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~HiddenViewsVisible.html)

[IDrawingDoc::IActiveDrawingView Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IActiveDrawingView.html)