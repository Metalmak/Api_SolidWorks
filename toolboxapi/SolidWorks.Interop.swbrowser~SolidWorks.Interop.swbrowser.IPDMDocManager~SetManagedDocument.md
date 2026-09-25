<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager~SetManagedDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| SetManagedDocument Method (IPDMDocManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) > [IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html) : SetManagedDocument Method (IPDMDocManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Document path and file name; the location in the vault does not need to be writable

Places the specified document under PDM management.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetManagedDocument( _    ByVal fileName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPDMDocManager Dim fileName As System.String Dim value As System.Boolean   value = instance.SetManagedDocument(fileName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetManagedDocument(     System.string fileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetManagedDocument(  &   System.String^ fileName ) ``` | |

#### Parameters

*fileName*
:   Document path and file name; the location in the vault does not need to be writable

#### Return Value

True if the managed document is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PDMDocManager::SetManagedDocument.

# ![](dotnetimages/collapse.gif)Remarks

Available only if you installed SOLIDWORKS Toolbox.

# ![](dotnetimages/collapse.gif)See Also

####

[IPDMDocManager Interface](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager.html)

[IPDMDocManager Members](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IPDMDocManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0