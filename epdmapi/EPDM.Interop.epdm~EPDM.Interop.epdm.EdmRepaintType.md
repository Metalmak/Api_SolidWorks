<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRepaintType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRepaintType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRepaintType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of flags passed into [IEdmImage::Reposition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~Reposition.html) to control how to handle repainting of the background window.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRepaintType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRepaintType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRepaintType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmRepaint\_Erase** | 2 = Trigger both paint and erase (WM\_ERASEBKGND) message |
| **EdmRepaint\_Nothing** | 0 = Do not refresh the window |
| **EdmRepaint\_Repaint** | 1 = Trigger a repaint (WM\_PAINT) message but not a background erase |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)