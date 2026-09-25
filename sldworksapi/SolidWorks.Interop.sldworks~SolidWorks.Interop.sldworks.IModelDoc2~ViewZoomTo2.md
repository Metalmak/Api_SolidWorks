<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomTo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ViewZoomTo2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ViewZoomTo2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X1*
:   X value for the lower-left point of the zoom area

*Y1*
:   Y value for the lower- left point of the zoom area

*Z1*
:   Z value for the lower-left point of the zoom area

*X2*
:   X value for the upper-right point of the zoom area

*Y2*
:   Y value for the upper-right point of the zoom area

*Z2*
:   Z value for the upper-right point of the zoom area

Zooms to the specified region.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ViewZoomTo2( _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double   instance.ViewZoomTo2(X1, Y1, Z1, X2, Y2, Z2) ``` | |

| C# |  |
| --- | --- |
| ``` void ViewZoomTo2(     System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ViewZoomTo2(  &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X1*
:   X value for the lower-left point of the zoom area

*Y1*
:   Y value for the lower- left point of the zoom area

*Z1*
:   Z value for the lower-left point of the zoom area

*X2*
:   X value for the upper-right point of the zoom area

*Y2*
:   Y value for the upper-right point of the zoom area

*Z2*
:   Z value for the upper-right point of the zoom area

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ViewZoomTo2.

# ![](dotnetimages/collapse.gif)Example

[Zoom To Region (VBA)](Zoom_to_Region_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::ViewZoomin Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomin.html)

[IModelDoc2::ViewZoomout Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomout.html)

[IModelDoc2::ViewZoomto Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomto.html)

[IModelDoc2::ViewZoomtofit2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomtofit2.html)

[IModelDoc2::ViewZoomToSelection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomToSelection.html)

[IModelDoc2::ViewOrientationUndo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewOrientationUndo.html)

[IModelDoc2::ViewRotate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotate.html)

[IModelDoc2::ViewRotateminusx Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusx.html)

[IModelDoc2::ViewRotateminusy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusy.html)

[IModelDoc2::ViewRotateminusz Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusz.html)

[IModelDoc2::ViewRotateplusx Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusx.html)

[IModelDoc2::ViewRotateplusy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusy.html)

[IModelDoc2::ViewRotateplusz Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusz.html)

[IModelDoc2::ViewRotXMinusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotXMinusNinety.html)

[IModelDoc2::ViewRotXPlusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotXPlusNinety.html)

[IModelDoc2::ViewRotYMinusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotYMinusNinety.html)

[IModelDoc2::ViewRotYPlusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotYPlusNinety.html)

[IModelDocExtension::ViewZoomToSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ViewZoomToSheet.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0