<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVEnableFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| EMVEnableFeatures Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : EMVEnableFeatures Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Enable features. Bitmask.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum EMVEnableFeatures     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As EMVEnableFeatures ``` | |

| C# |  |
| --- | --- |
| ``` public enum EMVEnableFeatures : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EMVEnableFeatures : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **eMVDisableGradientBackground** | 65536 = Changes the eDrawings Viewer background from a gradient to solid color |
| **eMVDisableMeasure** | 32768 = Disables measure |
| **eMVDisableMenuSave** | 8 = Disable the Save selection on the File menu (Complete UI mode) |
| **eMVDisableSNLCheckout** | 8192 = Disable SNL checkout  NOTE: If you disable SNL checkout, eDrawings Professional features may be disabled even if the document is review-enabled or if the eDrawings Professional license is present. |
| **eMVEnableSilentMode** | 16384 = Disable all dialogs |
| **eMVEnableUICommands** | 4194304 = When eDrawings is run as a COM object, user-interface (UI) commands are enabled |
| **eMVFullUI** | 16 = Display in Complete UI mode (preferred ) |
| **eMVHLR** | 256 = Display files saved in HLR (Hidden Lines Removed) display mode in HLR display mode |
| **eMVReadOnly** | 64 = Open the file as read only |
| **eMVSeparateMarkup** | 128 = Open all markup files associated with this file |
| **eMVSimplifiedUI** | 32 = Display in Simple UI mode |
| **eMVSmallToolbarButtons** | 2048 = Display Small toolbar buttons |
| **eMVSuppressMarkupFileOpen** | 4 = Do not display the File, Markup Open dialog |
| **eMVSuppressMarkupOpenMenu** | 512 = Disable the Open Markup selection on the File menu |
| **eMVSuppressRMBMenu** | 1024 = Disable the right-mouse button menu |
| **eMVSuppressSavePrompt** | 2 = Do not display the Save dialog even if the file was modified |
| **eMVSupressMenuBar** | 4096 = Hide the Menu toolbar |
| **eMVTriad** | 1 = Display triad |

# ![](dotnetimages/collapse.gif)See Also

####

[eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html)