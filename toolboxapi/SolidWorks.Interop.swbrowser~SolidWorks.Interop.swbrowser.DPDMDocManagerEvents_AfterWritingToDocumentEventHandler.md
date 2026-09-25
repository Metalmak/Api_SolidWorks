<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.DPDMDocManagerEvents_AfterWritingToDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| DPDMDocManagerEvents\_AfterWritingToDocumentEventHandler Delegate (SolidWorks.Interop.swbrowser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) : DPDMDocManagerEvents\_AfterWritingToDocumentEventHandler Delegate (SolidWorks.Interop.swbrowser) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Path and file name of document written to

Handles the notification that the specified PDM-managed document was written to.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPDMDocManagerEvents_AfterWritingToDocumentEventHandler( _    ByVal fileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPDMDocManagerEvents_AfterWritingToDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_AfterWritingToDocumentEventHandler(     System.string fileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPDMDocManagerEvents_AfterWritingToDocumentEventHandler(  &   System.String^ fileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndC%2B%2BCLI.html).

#### Parameters

*fileName*
:   Path and file name of document written to

# ![](dotnetimages/collapse.gif)Visual Basic Application (VBA) Syntax

See AfterWritingToDocument Event (PDMDocManager).

# ![](dotnetimages/collapse.gif)Example

See [Getting Started](GettingStarted-toolboxapi.html) for more information.

# ![](dotnetimages/collapse.gif)Remarks

Available only if you installed SOLIDWORKS Toolbox.

In the body of this handler, you can perform PDM document management functions such as:

* Determine the availability of fileName in the SOLIDWORKS Toolbox.* Copy a working file to the PDM-managed location, overwriting the PDM-managed version if necessary.* Set the read-only attribute of the PDM-managed file.

Before returning from this handler, you must call [IPDMDocManager::SetDocumentStatus](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetDocumentStatus.html) with [swPDMStatus\_e.swPDMStatusKnownAndAvailable](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html) in order to not generate an error.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0