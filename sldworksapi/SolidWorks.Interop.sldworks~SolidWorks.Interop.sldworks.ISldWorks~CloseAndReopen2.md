<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseAndReopen2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CloseAndReopen2 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : CloseAndReopen2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Doc*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html); drawing document to close and reopen

*Option*
:   Reopen options as defined in swCloseReopenOption\_e

*NewDoc*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html); reopened drawing document

Closes and reopens the specified drawing document without unloading its references from memory.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CloseAndReopen2( _    ByVal Doc As System.Object, _    ByVal Option As System.Integer, _    ByRef NewDoc As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Doc As System.Object Dim Option As System.Integer Dim NewDoc As System.Object Dim value As System.Integer   value = instance.CloseAndReopen2(Doc, Option, NewDoc) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CloseAndReopen2(     System.object Doc,    System.int Option,    out System.object NewDoc ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CloseAndReopen2(  &   System.Object^ Doc, &   System.int Option, &   [Out] System.Object^ NewDoc ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Doc*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html); drawing document to close and reopen

*Option*
:   Reopen options as defined in swCloseReopenOption\_e

*NewDoc*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html); reopened drawing document

#### Return Value

Error code as defined in swCloseReopenError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::CloseAndReopen2.

# ![](dotnetimages/collapse.gif)Example

Contact SOLIDWORKS API Support to obtain **Close and Reopen a Drawing Document (VBA, VB.NET, C#)**.

# ![](dotnetimages/collapse.gif)Remarks

Before a third-party application can process a drawing document that is open in SOLIDWORKS, it must close the document. Usually when a drawing document is closed, its references are unloaded from memory, and reopening the drawing document takes a lot of time. This method closes a drawing document, keeps its references in memory, and quickly reopens it.

After the drawing document is closed and before it is reopened, SOLIDWORKS fires a [FileCloseNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_FileCloseNotifyEventHandler.html) event with reason swFileCloseNotifyReason\_e.swFileCloseNotifyReason\_CloseForReload. In the handler of this event, a third-party application can call [ISldWorks::SetPromptFileName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetPromptFilename2.html) to open a different file, or it can process the specified document before it is reopened in SOLIDWORKS.

See [IModelDoc2::ReloadOrReplace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ReloadOrReplace.html) to perform a similar function with part and assembly documents.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::CloseAllDocuments Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseAllDocuments.html)

[ISldWorks::CloseDoc Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CloseDoc.html)

[ISldWorks::QuitDoc Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~QuitDoc.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30