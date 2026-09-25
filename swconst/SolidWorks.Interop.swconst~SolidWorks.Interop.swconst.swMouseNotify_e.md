<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swMouseNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swMouseNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swMouseNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Mouse notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swMouseNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swMouseNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swMouseNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swMouseNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMouseLBtnDblClkNotify** | 9 = MouseLBtnDblClkNotify |
| **swMouseLBtnDownNotify** | 3 = MouseLBtnDownNotify |
| **swMouseLBtnUpNotify** | 4 = MouseLBtnUpNotify |
| **swMouseMBtnDblClkNotify** | 11 = MouseMBtnDblClkNotify |
| **swMouseMBtnDownNotify** | 7 = MouseMBtnDownNotify |
| **swMouseMBtnUpNotify** | 8 = MouseMBtnUpNotify |
| **swMouseMoveNotify** | 2 = MouseMoveNotify |
| **swMouseNotify** | 1 = MouseNotify |
| **swMouseRBtnDblClkNotify** | 10 = MouseRBtnDblClkNotify |
| **swMouseRBtnDownNotify** | 5 = MouseRBtnDownNotify |
| **swMouseRBtnUpNotify** | 6 = MouseRBtnUpNotify |
| **swMouseSelectNotify** | 12 = MouseSelectNotify |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports mouse events (e.g., Mouse.h), include:

DECLARE\_REGISTRY\_RESOURCEID(IDR\_MOUSE)

BEGIN\_SINK\_MAP(CMouse)

SINK\_ENTRY\_EX(ID\_MOUSE\_EVENTS, DIID\_DMouseEvents, swMouseMoveNotify, MouseMoveNotify)

SINK\_ENTRY\_EX(ID\_MOUSE\_EVENTS, DIID\_DMouseEvents, swMouseSelectNotify, MouseSelectNotify)

SINK\_ENTRY\_EX(ID\_MOUSE\_EVENTS, DIID\_DMouseEvents, swMouseLBtnDownNotify, MouseLBtnDownNotify)

END\_SINK\_MAP()

If developing a C++ application, use these enumerators to register for notifications for the IMouse events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)