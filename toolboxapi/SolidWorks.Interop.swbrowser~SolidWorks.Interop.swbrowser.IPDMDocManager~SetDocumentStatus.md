<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager~SetDocumentStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| SetDocumentStatus Method (IPDMDocManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) > [IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html) : SetDocumentStatus Method (IPDMDocManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*status*
:   Document status as defined in [swPDMStatus\_e](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html)

Sets the status of the currently active PDM document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDocumentStatus( _    ByVal status As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPDMDocManager Dim status As System.Integer Dim value As System.Boolean   value = instance.SetDocumentStatus(status) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDocumentStatus(     System.int status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDocumentStatus(  &   System.int status ) ``` | |

#### Parameters

*status*
:   Document status as defined in [swPDMStatus\_e](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html)

#### Return Value

True if the document status is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PDMDocManager::SetDocumentStatus.

# ![](dotnetimages/collapse.gif)Remarks

Available only if you installed SOLIDWORKS Toolbox.

# ![](dotnetimages/collapse.gif)See Also

####

[IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html)

[IPDMDocManager Members](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0