<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.DPDMDocManagerEvents_NewDocumentAddedEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| DPDMDocManagerEvents\_NewDocumentAddedEventHandler Delegate (SolidWorks.Interop.swbrowser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) : DPDMDocManagerEvents\_NewDocumentAddedEventHandler Delegate (SolidWorks.Interop.swbrowser) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Path and file name of the new part

*ToolboxID*
:   ID is calculated for copied part creation; otherwise 1

*AddedToBrowser*
:   True if the the part resides in the SOLIDWORKS Toolbox database, false if not

Handles the notification that the specified part was added to the Toolbox.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPDMDocManagerEvents_NewDocumentAddedEventHandler( _    ByVal fileName As System.String, _    ByVal ToolboxID As System.Integer, _    ByVal AddedToBrowser As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPDMDocManagerEvents_NewDocumentAddedEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_NewDocumentAddedEventHandler(     System.string fileName,    System.int ToolboxID,    System.int AddedToBrowser ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_NewDocumentAddedEventHandler(  &   System.String^ fileName, &   System.int ToolboxID, &   System.int AddedToBrowser ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndC%2B%2BCLI.html).

#### Parameters

*fileName*
:   Path and file name of the new part

*ToolboxID*
:   ID is calculated for copied part creation; otherwise 1

*AddedToBrowser*
:   True if the the part resides in the SOLIDWORKS Toolbox database, false if not

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See NewDocumentAdded Event (PDMDocManager).

# ![](dotnetimages/collapse.gif)Example

See [Getting Started](GettingStarted-toolboxapi.html) for more information.

# ![](dotnetimages/collapse.gif)Remarks

In this handler, call [IPDMDocManager:SetManagedDocument](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetManagedDocument.html) to direct the Toolbox Browser application to use the new document. For copied parts, the file inserted into the assembly is the IPDMDocManager::SetManagedDocument filename.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0