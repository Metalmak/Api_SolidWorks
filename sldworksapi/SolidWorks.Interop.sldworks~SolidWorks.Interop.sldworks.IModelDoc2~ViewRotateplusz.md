<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusz.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ViewRotateplusz Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ViewRotateplusz Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Rotates the view around z in a positive direction with the current increment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ViewRotateplusz() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2   instance.ViewRotateplusz() ``` | |

| C# |  |
| --- | --- |
| ``` void ViewRotateplusz() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ViewRotateplusz(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ViewRotateplusz.

# ![](dotnetimages/collapse.gif)Example

[Rotate Model (VBA)](Rotate_Model_Example_VB.htm)

[Rotate Model (VB.NET)](Rotate_Model_Example_VBNET.htm)

[Rotate Model (C#)](Rotate_Model_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To increase the speed of dynamic view changes with hidden-edge display or hidden-grey display, use [IModelView::StartDynamics](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~StartDynamics.html) and [IModelView::StopDynamics](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~StopDynamics.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::ViewZoomToSelection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomToSelection.html)

[IModelDoc2::ViewZoomtofit2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomtofit2.html)

[IModelDoc2::ViewZoomTo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomTo2.html)

[IModelDoc2::ViewZoomto Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomto.html)

[IModelDoc2::ViewZoomout Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomout.html)

[IModelDoc2::ViewZoomin Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomin.html)

[IModelDoc2::ViewRotYPlusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotYPlusNinety.html)

[IModelDoc2::ViewRotYMinusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotYMinusNinety.html)

[IModelDoc2::ViewRotXPlusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotXPlusNinety.html)

[IModelDoc2::ViewRotXMinusNinety Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotXMinusNinety.html)

[IModelDoc2::ViewRotateplusy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusy.html)

[IModelDoc2::ViewRotateplusx Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateplusx.html)

[IModelDoc2::ViewRotateminusz Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusz.html)

[IModelDoc2::ViewRotateminusy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusy.html)

[IModelDoc2::ViewRotateminusx Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotateminusx.html)

[IModelDoc2::ViewRotate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewRotate.html)

[IModelDoc2::ViewOrientationUndo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewOrientationUndo.html)

[IModelDoc2::ViewZoomto Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewZoomto.html)

[IModelDocExtension::ViewZoomToSheet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ViewZoomToSheet.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0