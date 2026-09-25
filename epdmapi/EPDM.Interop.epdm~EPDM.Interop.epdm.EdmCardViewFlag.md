<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmCardViewFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCardViewFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for appearance and functionality of card views created with [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html) and [IEdmFolder10::CreateCardView2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10~CreateCardView2.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmCardViewFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmCardViewFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmCardViewFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmCvf\_3StateCheckboxes** | 2 = Permit three-state checkboxes |
| **EdmCvf\_CallSaveOnCtrlReturn** | 512 = Save on CTRL-Enter |
| **EdmCvf\_ComputeDefaultValues** | 8 = Compute default values in the card |
| **EdmCvf\_DisableButtons** | 256 = Disable all buttons in the card |
| **EdmCvf\_Normal** | 253 = Default (1+4+8+16+32+64+128) |
| **EdmCvf\_Nothing** | 0 = Nothing |
| **EdmCvf\_PermitComputedValues** | 64 = Permit controls to receive values from input formulas |
| **EdmCvf\_PermitControlledTabs** | 1 = Permit controlling tab controls with variables |
| **EdmCvf\_PermitReadOnlyFields** | 32 = Permit the card to have read-only fields |
| **EdmCvf\_RunFormulas** | 4 = Evaluate input formulas in the card |
| **EdmCvf\_RunFormulasOnOpen** | 1024 = Force execution of formulas on all controls when opened |
| **EdmCvf\_SearchMode** | 130 = Search tool mode (2+128) |
| **EdmCvf\_SerNoMenu** | 1048576 = Show shortcut menu for serial numbers |
| **EdmCvf\_TextureBackground** | 128 = Fade the card background |
| **EdmCvf\_VerifyValues** | 16 = Check mandatory and unique values during save |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)