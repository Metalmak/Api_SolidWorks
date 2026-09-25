<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefreshFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRefreshFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRefreshFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags that cause SOLIDWORKS PDM Professional to refresh elements of the user interface. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRefreshFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRefreshFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRefreshFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmRefresh\_FileList** | 1 = Refresh the file listing in File Explorer; this value should be returned if you add, delete, rename, check out, check in, etc., a file and want the change to be immediately visible to the user |
| **EdmRefresh\_Hooks** | 2 = Force reloading of hooks; this value is normally only returned if your add-in changes the number of registered hooks |
| **EdmRefresh\_Menu** | 4 = Force an update of the Tools menu in the File Explorer; this value is normally only returned if your add-in changes the number of registered menu commands |
| **EdmRefresh\_Nothing** | 0 = No refresh is required |
| **EdmRefresh\_Toolbar** | 8 = Force an update of the toolbar in File Explorer; this value is normally only returned if your add-in changes the number of registered menu commands with toolbar buttons |

# ![](dotnetimages/collapse.gif)Remarks

You can return a combination of these flags from your add-in's [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) via the [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html) struct to cause SOLIDWORKS PDM Professional to refresh certain parts of the user interface.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[EdmCmd::mlEdmRefreshFlags Field](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd~mlEdmRefreshFlags.html)