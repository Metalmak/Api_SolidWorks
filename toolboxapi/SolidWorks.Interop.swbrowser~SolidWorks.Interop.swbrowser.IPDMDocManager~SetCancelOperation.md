<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager~SetCancelOperation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| SetCancelOperation Method (IPDMDocManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) > [IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html) : SetCancelOperation Method (IPDMDocManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*cancelOp*
:   True to cancel the current operation, false to continue the operation

Cancels the current operation after any notifications are returned.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCancelOperation( _    ByVal cancelOp As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPDMDocManager Dim cancelOp As System.Integer Dim value As System.Boolean   value = instance.SetCancelOperation(cancelOp) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetCancelOperation(     System.int cancelOp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetCancelOperation(  &   System.int cancelOp ) ``` | |

#### Parameters

*cancelOp*
:   True to cancel the current operation, false to continue the operation

#### Return Value

True if the current operation is canceled, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PDMDocManager::SetCancelOperation.

# ![](dotnetimages/collapse.gif)Remarks

Available only if you installed SOLIDWORKS Toolbox.

# ![](dotnetimages/collapse.gif)See Also

####

[IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html)

[IPDMDocManager Members](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0