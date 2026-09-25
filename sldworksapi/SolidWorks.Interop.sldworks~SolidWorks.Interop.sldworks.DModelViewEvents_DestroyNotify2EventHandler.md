<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DModelViewEvents_DestroyNotify2EventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DModelViewEvents\_DestroyNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DModelViewEvents\_DestroyNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DestroyType*
:   Value as defined by swDestroyNotifyType\_e

Pre-notifies the user program when a model view is about to be destroyed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DModelViewEvents_DestroyNotify2EventHandler( _    ByVal DestroyType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DModelViewEvents_DestroyNotify2EventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_DestroyNotify2EventHandler(     System.int DestroyType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_DestroyNotify2EventHandler(  &   System.int DestroyType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DestroyType*
:   Value as defined by swDestroyNotifyType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DestroyNotify2 Event (ModelView).

# ![](dotnetimages/collapse.gif)Remarks

This event is sent when a view is being destroyed and will no longer be available to the end-user. In this case, the destroyType value is swDestroyNotifyDestroy.

This event is also sent for each view of a model when the document is closed, yet the view is not destroyed. This can happen when the model is being used by an open assembly or drawing document. In this case, the destroyType value is swDestroyNotifyHidden. This indicates that the view is still available for use, but is not visible.

If the part is then reopened, a IPartDoc [ViewNewNotify2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_ViewNewNotify2EventHandler.html) event is again sent for all views in the part. At this point, you can recreate your link to these views, or if your application did not destroy the views, you can recognize that these views are no longer hidden. When the document and all referencing assemblies and drawings are finally closed, then the views are destroyed and this event is sent for each of the model views, with the destroyType = swDestroyNotifyDestroy.

If developing a C++ application, use swViewDestroyNotify2 to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0