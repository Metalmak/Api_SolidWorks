<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DModelViewEvents_PerspectiveViewNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DModelViewEvents\_PerspectiveViewNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DModelViewEvents\_PerspectiveViewNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Left*
:   Coordinate of the left vertical clipping plane

*Right*
:   Coordinate of the right vertical clipping plane

*bottom*
:   Coordinate of the bottom horizontal clipping plane

*Top*
:   Coordinate of the top horizontal clipping plane

*zNear*
:   Distance to the near depth clipping plane

*zFar*
:   Distance to the far depth clipping plane

Post-notifies the user program when the perspective view is changed (for example, if the user rotates the perspective view).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DModelViewEvents_PerspectiveViewNotifyEventHandler( _    ByVal Left As System.Double, _    ByVal Right As System.Double, _    ByVal bottom As System.Double, _    ByVal Top As System.Double, _    ByVal zNear As System.Double, _    ByVal zFar As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DModelViewEvents_PerspectiveViewNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_PerspectiveViewNotifyEventHandler(     System.double Left,    System.double Right,    System.double bottom,    System.double Top,    System.double zNear,    System.double zFar ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_PerspectiveViewNotifyEventHandler(  &   System.double Left, &   System.double Right, &   System.double bottom, &   System.double Top, &   System.double zNear, &   System.double zFar ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Left*
:   Coordinate of the left vertical clipping plane

*Right*
:   Coordinate of the right vertical clipping plane

*bottom*
:   Coordinate of the bottom horizontal clipping plane

*Top*
:   Coordinate of the top horizontal clipping plane

*zNear*
:   Distance to the near depth clipping plane

*zFar*
:   Distance to the far depth clipping plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PerspectiveViewNotify Event (ModelView).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swViewPerspectiveViewNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0