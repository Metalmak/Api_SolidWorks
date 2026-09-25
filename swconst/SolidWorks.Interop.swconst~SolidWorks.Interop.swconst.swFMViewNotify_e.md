<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFMViewNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFMViewNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFMViewNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

FeatureManager design tree notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFMViewNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFMViewNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFMViewNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFMViewNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFMViewActivateNotify** | 1 = ActivateNotify |
| **swFMViewDeactivateNotify** | 2 = DeactivateNotify |
| **swFMViewDestroyNotify** | 3 = DestroyNotify |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports FeatureManager design tree events (e.g., FeatMgrView.h), include:

DECLARE\_REGISTRY\_RESOURCEID(IDR\_FeatMgrView)

BEGIN\_SINK\_MAP(CFeatMgrView)

SINK\_ENTRY\_EX(ID\_FEATMGRVIEW\_EVENTS, DIID\_DFeatMgrViewEvents, swFMViewDestroyNotify , DestroyNotify)

SINK\_ENTRY\_EX(ID\_FEATMGRVIEW\_EVENTS, DIID\_DFeatMgrViewEvents, swFMViewActivateNotify, ActivateNotify)

SINK\_ENTRY\_EX(ID\_FEATMGRVIEW\_EVENTS, DIID\_DFeatMgrViewEvents, swFMViewDeactivateNotify , DeActivateNotify)

END\_SINK\_MAP()

If developing a C++ application, use these enumerators to register for notifications for IFeatMgrView events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)