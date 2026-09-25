<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSWPropertySheetEvents_CreateControlNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSWPropertySheetEvents\_CreateControlNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSWPropertySheetEvents\_CreateControlNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PageIndex*
:   Index of property page within the property sheet for the add-in (see **Remarks**)

*ControlDispatch*
:   ActiveX control

Fired when the ActiveX control is created on the property page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSWPropertySheetEvents_CreateControlNotifyEventHandler( _    ByVal PageIndex As System.Integer, _    ByVal ControlDispatch As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSWPropertySheetEvents_CreateControlNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSWPropertySheetEvents_CreateControlNotifyEventHandler(     System.int PageIndex,    System.object ControlDispatch ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSWPropertySheetEvents_CreateControlNotifyEventHandler(  &   System.int PageIndex, &   System.Object^ ControlDispatch ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PageIndex*
:   Index of property page within the property sheet for the add-in (see **Remarks**)

*ControlDispatch*
:   ActiveX control

#### Return Value

ActiveX control

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CreateControlNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

If PageIndex is the same index as returned by [ISWPropertySheet::AddActivePage](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISWPropertySheet~AddActivePage.html), then ControlDispatch will contain the Dispatch pointer of the ActiveX control.

If developing a C++ application, use swPropertySheetCreateControlNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP5, Revision Number 12.5