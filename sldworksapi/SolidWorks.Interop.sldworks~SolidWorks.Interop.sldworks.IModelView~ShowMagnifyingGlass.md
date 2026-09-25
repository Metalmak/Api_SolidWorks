<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~ShowMagnifyingGlass.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowMagnifyingGlass Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : ShowMagnifyingGlass Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Ptx*
:   x coordinate

*Pty*
:   y coordinate

*Ptz*
:   z coordinate

*ZoomFactor*
:   Zoom factor

*HideOnClick*
:   True to hide the Magnifying Glass tool when the mouse is right-clicked, false to not

*FollowMouse*
:   True to have the Magnifying Glass tool follow the pointer, false to not

Shows the Magnifying Glass tool at the specified coordinates.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowMagnifyingGlass( _    ByVal Ptx As System.Double, _    ByVal Pty As System.Double, _    ByVal Ptz As System.Double, _    ByVal ZoomFactor As System.Double, _    ByVal HideOnClick As System.Boolean, _    ByVal FollowMouse As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim Ptx As System.Double Dim Pty As System.Double Dim Ptz As System.Double Dim ZoomFactor As System.Double Dim HideOnClick As System.Boolean Dim FollowMouse As System.Boolean   instance.ShowMagnifyingGlass(Ptx, Pty, Ptz, ZoomFactor, HideOnClick, FollowMouse) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowMagnifyingGlass(     System.double Ptx,    System.double Pty,    System.double Ptz,    System.double ZoomFactor,    System.bool HideOnClick,    System.bool FollowMouse ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowMagnifyingGlass(  &   System.double Ptx, &   System.double Pty, &   System.double Ptz, &   System.double ZoomFactor, &   System.bool HideOnClick, &   System.bool FollowMouse ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Ptx*
:   x coordinate

*Pty*
:   y coordinate

*Ptz*
:   z coordinate

*ZoomFactor*
:   Zoom factor

*HideOnClick*
:   True to hide the Magnifying Glass tool when the mouse is right-clicked, false to not

*FollowMouse*
:   True to have the Magnifying Glass tool follow the pointer, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::ShowMagnifyingGlass.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

'----------------------------------------
'
' Preconditions: Model document is open.
'
' Postconditions: None
'
'----------------------------------------
Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelView As SldWorks.ModelView
Sub main()

Set swApp = Application.SldWorks
Set swModel = swApp.**ActiveDoc**
Set swModelView = swModel.**ActiveView**

swModelView.**ShowMagnifyingGlass** -0.01928933522023, 0.004431675106825, -0.001816629754713, 2, True, True
swModelView.**MoveMagnifyingGlass** -0.01928933522023, 0.004431675106825, -0.004
swModelView.**MoveMagnifyingGlass** -0.01928933522023, 0.004431675106825, -0.016
swModelView.**HideMagnifyingGlass**

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelView::HideMagnifyingGlass Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~HideMagnifyingGlass.html)

[IModelView::MoveMagnifyingGlass Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~MoveMagnifyingGlass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0