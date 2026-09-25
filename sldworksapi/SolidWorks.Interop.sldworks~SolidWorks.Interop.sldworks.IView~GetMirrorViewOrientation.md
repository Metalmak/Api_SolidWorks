<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetMirrorViewOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetMirrorViewOrientation Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetMirrorViewOrientation Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BIsMirrorView*
:   True if the view is mirrored, false if not

*LMirrorViewOrientation*
:   Orientation of the mirror view as defined in swMirrorViewPositions\_e

Gets whether this view is mirrored.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMirrorViewOrientation( _    ByRef BIsMirrorView As System.Boolean, _    ByRef LMirrorViewOrientation As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim BIsMirrorView As System.Boolean Dim LMirrorViewOrientation As System.Integer Dim value As System.Boolean   value = instance.GetMirrorViewOrientation(BIsMirrorView, LMirrorViewOrientation) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetMirrorViewOrientation(     out System.bool BIsMirrorView,    out System.int LMirrorViewOrientation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetMirrorViewOrientation(  &   [Out] System.bool BIsMirrorView, &   [Out] System.int LMirrorViewOrientation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BIsMirrorView*
:   True if the view is mirrored, false if not

*LMirrorViewOrientation*
:   Orientation of the mirror view as defined in swMirrorViewPositions\_e

#### Return Value

True if the method executed successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetMirrorViewOrientation.

# ![](dotnetimages/collapse.gif)Example

[Mirror View (C#)](Mirror_View_Example_CSharp.htm)

[Mirror View (VB.NET)](Mirror_View_Example_VBNET.htm)

[Mirror View (VBA)](Mirror_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IViewe::SetMirrorViewOrientation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetMirrorViewOrientation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0