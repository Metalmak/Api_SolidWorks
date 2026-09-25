<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~GenerateItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GenerateItems Method (IEdmBatchItemGeneration) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchItemGeneration Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html) : GenerateItems Method (IEdmBatchItemGeneration) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*ppoRetItems*
:   Array of [EdmGenItemInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo.html) structures, one structure for each new item

*pbOpen*
:   True, if the following occurred:

    * [EdmItemGenerationFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemGenerationFlags.html).Eigcf\_OpenItemsCheckbox was set in [IEdmBatchItemGeneration::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~CreateTree.html).* The user selected the checkbox to open items after creation in the dialog box displayed by [IEdmBatchItemGeneration::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~ShowDlg.html).

    False, if not

*poCallback*
:   Null; reserved for future use

Creates the items added to the batch by [IEdmBatchItemGeneration::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~AddSelection.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GenerateItems( _    ByVal lParentWnd As System.Integer, _    ByRef ppoRetItems() As EdmGenItemInfo, _    ByRef pbOpen As System.Boolean, _    Optional ByVal poCallback As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GenerateItems(     System.int lParentWnd,    out EdmGenItemInfo[] ppoRetItems,    out System.bool pbOpen,    System.object poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GenerateItems(  &   System.int lParentWnd, &   [Out] array<EdmGenItemInfo>^ ppoRetItems, &   [Out] System.bool pbOpen, &   System.Object^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*ppoRetItems*
:   Array of [EdmGenItemInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGenItemInfo.html) structures, one structure for each new item

*pbOpen*
:   True, if the following occurred:

    * [EdmItemGenerationFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemGenerationFlags.html).Eigcf\_OpenItemsCheckbox was set in [IEdmBatchItemGeneration::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~CreateTree.html).* The user selected the checkbox to open items after creation in the dialog box displayed by [IEdmBatchItemGeneration::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~ShowDlg.html).

    False, if not

*poCallback*
:   Null; reserved for future use

# ![](dotnetimages/collapse.gif)Example

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchItemGeneration Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html)

[IEdmBatchItemGeneration Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010