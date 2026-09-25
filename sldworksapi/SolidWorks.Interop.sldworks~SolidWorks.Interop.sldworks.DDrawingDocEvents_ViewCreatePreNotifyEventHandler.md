<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_ViewCreatePreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_ViewCreatePreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_ViewCreatePreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*modelDocBeingAdded*
:   [Model document](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) used to create the drawing view

Pre-notifies the user application when a drawing view is about to be created.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_ViewCreatePreNotifyEventHandler( _    ByVal modelDocBeingAdded As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_ViewCreatePreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ViewCreatePreNotifyEventHandler(     System.object modelDocBeingAdded ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ViewCreatePreNotifyEventHandler(  &   System.Object^ modelDocBeingAdded ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*modelDocBeingAdded*
:   [Model document](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) used to create the drawing view

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ViewCreatePreNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Remarks

This notification occurs just before the drawing view is added as a feature to the drawing document. Use [IModelDoc2::GetPathName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) and [IConfigurationManager::ActiveConfiguration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html) to get the model document's path, filename, and configuration to use to create the drawing view.

This notification also gets fired for empty drawing views. Because empty drawing views do not have a model document, the argument ModelDocBeingAdded is NULL or Nothing. Use the event handler to check ModelDocBeingAdded for NULL or Nothing before using this notification.

If developing a C++ application, then use swDrawingViewCreatePreNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0