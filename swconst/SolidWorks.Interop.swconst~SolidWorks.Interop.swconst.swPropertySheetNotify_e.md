<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPropertySheetNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPropertySheetNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPropertySheetNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Property sheet notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPropertySheetNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPropertySheetNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPropertySheetNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPropertySheetNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPropertySheetCreateControlNotify** | 5 = CreateControlNotify |
| **swPropertySheetDestroyNotify** | 1 = DestroyNotify |
| **swPropertySheetHelpNotify** | 2 = HelpNotify |
| **swPropertySheetOnCancelNotify** | 4 = OnCancelNotify |
| **swPropertySheetOnOKNotify** | 3 = OnOKNotify |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports property sheet events ( e.g., SwPropertySheet.h), include:

BEGIN\_SINK\_MAP(CSwPropertySheet)

SINK\_ENTRY\_EX(ID\_SWPROPERTYSHEET\_EVENTS, DIID\_DSwPropertySheetEvents, swPropertySheetCreateControlNotify, CreateControlNotify)

SINK\_ENTRY\_EX(ID\_SWPROPERTYSHEET\_EVENTS, DIID\_DSwPropertySheetEvents, swPropertySheetDestroyNotify, DestroyNotify)

END\_SINK\_MAP()

If developing a C++ application, use these enumerators to register for notifications for ISWPropertySheet events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)