<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DModelViewEvents_ViewChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DModelViewEvents\_ViewChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DModelViewEvents\_ViewChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*View*
:   See **Remarks**

Post-notifies the user program when a view is altered and returns the new transform matrix of the view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DModelViewEvents_ViewChangeNotifyEventHandler( _    ByVal View As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DModelViewEvents_ViewChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_ViewChangeNotifyEventHandler(     System.object View ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_ViewChangeNotifyEventHandler(  &   System.Object^ View ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*View*
:   See **Remarks**

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ViewChangeNotify Event (ModelView).

# ![](dotnetimages/collapse.gif)Remarks

In Visual Basic for Applications (VBA), the view argument is a VARIANT of type SafeArray of 16 doubles:

|  |  |
| --- | --- |
| **Elements** | **Values** |
| First 9 | Standard 3x3 rotation matrix |
| Next 3 | Define translation |
| Next 1 | For scaling |
| Last 3 | Not used |

Your application is responsible for destroying the SafeArray when you are finished with it.

If developing a C++ application, use swViewChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0