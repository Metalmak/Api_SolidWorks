<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_FileNewPreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_FileNewPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_FileNewPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*
:   Document type as defined by swDocumentTypes\_e

*TemplateName*
:   Template path name or file extension

Fired before a new document is created either using the SOLIDWORKS API or the SOLIDWORKS user-interface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_FileNewPreNotifyEventHandler( _    ByVal DocType As System.Integer, _    ByVal TemplateName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_FileNewPreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_FileNewPreNotifyEventHandler(     System.int DocType,    System.string TemplateName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_FileNewPreNotifyEventHandler(  &   System.int DocType, &   System.String^ TemplateName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*
:   Document type as defined by swDocumentTypes\_e

*TemplateName*
:   Template path name or file extension

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FileNewPreNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

Creating a new document using the SOLIDWORKS user-interface includes:

* Clicking a document-type button on the New SOLIDWORKS Document dialog.

  * inserting a new component (part or assembly).

NOTE: This event is not raised when creating split parts.

You can cancel the creation of a new document by returning S\_FALSE(1) from the event handler.

If developing a C++ application, use swAppFileNewPreNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP4, Revision Number 15.4