<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetMirrorViewOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetMirrorViewOrientation Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : SetMirrorViewOrientation Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BSetIsMirrorView*
:   True to mirror the view, false to not

*BMirrorVieworientation*
:   Orientation of the mirror view as defined in swMirrorViewPositions\_e

Sets whether to mirror this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMirrorViewOrientation( _    ByVal BSetIsMirrorView As System.Boolean, _    ByVal BMirrorVieworientation As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim BSetIsMirrorView As System.Boolean Dim BMirrorVieworientation As System.Integer Dim value As System.Boolean   value = instance.SetMirrorViewOrientation(BSetIsMirrorView, BMirrorVieworientation) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetMirrorViewOrientation(     System.bool BSetIsMirrorView,    System.int BMirrorVieworientation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetMirrorViewOrientation(  &   System.bool BSetIsMirrorView, &   System.int BMirrorVieworientation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BSetIsMirrorView*
:   True to mirror the view, false to not

*BMirrorVieworientation*
:   Orientation of the mirror view as defined in swMirrorViewPositions\_e

#### Return Value

True if the method executed successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::SetMirrorViewOrientation.

# ![](dotnetimages/collapse.gif)Example

[Mirror View (C#)](Mirror_View_Example_CSharp.htm)

[Mirror View (VB.NET)](Mirror_View_Example_VBNET.htm)

[Mirror View (VBA)](Mirror_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetMirrorViewOrientation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetMirrorViewOrientation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0