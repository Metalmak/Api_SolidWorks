<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| ISwHtmlInterface Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) : ISwHtmlInterface Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Must be implemented in each add-in's Quick Tips HTML page so that users can interact with the add-in's Quick Tips and see associated Bubble ToolTips.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwHtmlInterface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwHtmlInterface ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwHtmlInterface ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface.

# ![](dotnetimages/collapse.gif)Example

[Show Bubble ToolTip (VBA)](Show_Bubble_ToolTip_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To access this API, include the following line of code in your application. See Quick Tips and Bubble ToolTips for more information.

CreateObject('SwHtmlControl.SwHtmlInterface')

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

[SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html)

ISldWorks::InstallQuickTipGuide

ISldWorks::RefreshQuickTipWindow

ISldWorks::UnInstallQuickTipGuide

ISwQuickTip