<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swViewNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swViewNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swViewNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Model view notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swViewNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swViewNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swViewNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swViewNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swViewBufferSwapNotify** | 5 = BufferSwapNotify |
| **swViewChangeNotify** | 2 = ViewChangeNotify |
| **swViewDestroyNotify** | Obsolete |
| **swViewDestroyNotify2** | 6 = DestroyNotify2 |
| **swViewDisplayModeChangePostNotify** | 13 = DisplayModeChangePostNotify |
| **swViewDisplayModeChangePreNotify** | 12 = DisplayModeChangePreNotify |
| **swViewGraphicsRenderPostNotify** | 11 = GraphicsRenderPostNotify |
| **swViewPerspectiveViewNotify** | 7 = PerspectiveViewNotify |
| **swViewPrintNotify** | Obsolete |
| **swViewPrintNotify2** | 14 = PrintNotify2 |
| **swViewRenderLayer0Notify** | 8 = RenderLayerNotify |
| **swViewRepaintNotify** | 1 = RepaintNotify |
| **swViewRepaintPostNotify** | 4 = RepaintPostNotify |
| **swViewUserClearSelectionsNotify** | 9 = UserClearSelectionsNotify |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports model view events (e.g., DocView.h), include:

BEGIN\_SINK\_MAP(CDocView)

SINK\_ENTRY\_EX(ID\_MODELVIEW\_EVENTS, DIID\_DModelViewEvents, swViewDestroyNotify, DestroyNotify)

SINK\_ENTRY\_EX(ID\_MODELVIEW\_EVENTS, DIID\_DModelViewEvents, swViewRepaintNotify, RepaintNotify)

END\_SINK\_MAP()

If developing a C++ application, use these enumerators to register for notifications for the IModelView events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)