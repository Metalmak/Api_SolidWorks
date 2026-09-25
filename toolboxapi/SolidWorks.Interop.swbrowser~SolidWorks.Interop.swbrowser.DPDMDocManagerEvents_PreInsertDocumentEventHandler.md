<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.DPDMDocManagerEvents_PreInsertDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| DPDMDocManagerEvents\_PreInsertDocumentEventHandler Delegate (SolidWorks.Interop.swbrowser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) : DPDMDocManagerEvents\_PreInsertDocumentEventHandler Delegate (SolidWorks.Interop.swbrowser) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Path and file name of the document to insert

*ToolboxID*
:   ID is calculated for copied part creation; otherwise 1

Handles the notification that the specified PDM-managed document is about to be inserted into an assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPDMDocManagerEvents_PreInsertDocumentEventHandler( _    ByVal fileName As System.String, _    ByVal ToolboxID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPDMDocManagerEvents_PreInsertDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_PreInsertDocumentEventHandler(     System.string fileName,    System.int ToolboxID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_PreInsertDocumentEventHandler(  &   System.String^ fileName, &   System.int ToolboxID ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndC%2B%2BCLI.html).

#### Parameters

*fileName*
:   Path and file name of the document to insert

*ToolboxID*
:   ID is calculated for copied part creation; otherwise 1

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See PreInsertDocument Event (PDMDocManager).

# ![](dotnetimages/collapse.gif)Example

See [Getting Started](GettingStarted-toolboxapi.html) for more information.

# ![](dotnetimages/collapse.gif)Remarks

Works like the SOLIDWORKS FileDropPreNotify event for the [SmartFastener](GettingStarted-toolboxapi.html#Insert). If a file with the same name is already open in SOLIDWORKS, Toolbox uses that file and does not send the PreInsertDocument notification.

Before returning from this handler, you must call [IPDMDocManager::SetManagedDocument](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetManagedDocument.html). The PDM application can use this method to direct the Toolbox Browser application to work with a file other than the PDM-managed document, which may not be writable. If the file does not exist, SOLIDWORKS generates an error and aborts all operations. If this file name is null for copied parts, SOLIDWORKS creates a new part. For all other insertions, SOLIDWORKS uses the original file name when an empty file name is specified.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0