<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemGenerationFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmItemGenerationFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmItemGenerationFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags that control the behavior of [IEdmBatchItemGeneration::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~CreateTree.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmItemGenerationFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmItemGenerationFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmItemGenerationFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Eigcf\_Nothing** | 0 = Default behavior |
| **Eigcf\_OpenItemsCheckbox** | 1 = This flag does not change the behavior of the IEdmBatchItemGeneration::CreateTree method itself, but it does affect a subsequent call to [IEdmBatchItemGeneration::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~ShowDlg.html); the dialog box displayed by IEdmBatchItemGeneration::ShowDlg will contain a checkbox to open items after the completion of the item-creation command if this flag is specified |

# ![](dotnetimages/collapse.gif)Remarks

See also the general note about items in the API.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)