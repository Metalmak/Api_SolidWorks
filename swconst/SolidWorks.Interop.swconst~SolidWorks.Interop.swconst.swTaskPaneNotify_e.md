<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTaskPaneNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swTaskPaneNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swTaskPaneNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Task Pane notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swTaskPaneNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swTaskPaneNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swTaskPaneNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swTaskPaneNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAppTaskPaneActivateNotify** | 1 = ActivateNotify |
| **swAppTaskPaneDeactivateNotify** | 2 = DeactivateNotify |
| **swAppTaskPaneDestroyNotify** | 3 = DestroyNotify |
| **swAppTaskPaneToolbarButtonClicked** | 4 = ToolbarButtonClicked |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports Task Pane events (e.g., Taskpane.h, include:

DECLARE\_REGISTRY\_RESOURCEID(IDR\_TaskPane)

BEGIN\_SINK\_MAP(CTaskPane)

SINK\_ENTRY\_EX(ID\_TASKPANE\_EVENTS, DIID\_DTaskpaneViewEvents, swAppTaskPaneDestroyNotify, DestroyNotify)

SINK\_ENTRY\_EX(ID\_TASKPANE\_EVENTS, DIID\_DTaskpaneViewEvents, swAppTaskPaneActivateNotify, ActivateNotify)

SINK\_ENTRY\_EX(ID\_TASKPANE\_EVENTS, DIID\_DTaskpaneViewEvents, swAppTaskPaneDeactivateNotify, DeActivateNotify)

END\_SINK\_MAP()

If developing a C++ application, use these enumerators to register for notifications for the ITaskpaneView events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)