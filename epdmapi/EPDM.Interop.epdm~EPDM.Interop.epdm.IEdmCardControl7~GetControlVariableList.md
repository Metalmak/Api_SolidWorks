<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl7~GetControlVariableList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetControlVariableList Method (IEdmCardControl7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl7.html) : GetControlVariableList Method (IEdmCardControl7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDocumentID*
:   ID of the file

*ppVariableItemsList*
:   Array of list values; empty if the card control is not associated with a list (see **Remarks**)

Gets the list values associated with this drop-down list card control.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetControlVariableList( _    ByVal lDocumentID As System.Integer, _    ByRef ppVariableItemsList() As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetControlVariableList(     System.int lDocumentID,    out System.string[] ppVariableItemsList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetControlVariableList(  &   System.int lDocumentID, &   [Out] System.array<String^>^ ppVariableItemsList ) ``` | |

#### Parameters

*lDocumentID*
:   ID of the file

*ppVariableItemsList*
:   Array of list values; empty if the card control is not associated with a list (see **Remarks**)

#### Return Value

True if retrieving the list is successful, false if not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardControl7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IEdmCardControl5::ControlType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~ControlType.html) is set to [EdmCardControlType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardControlType.html):

* EdmCtrl\_ComboboxDropdown* EdmCtrl\_ComboboxDroplist* EdmCtrl\_ComboboxSimple* EdmCtrl\_Listbox

This method supports the following items that appear in the **Admin tool > Card Editor** when you double-click on a droplist, dropdown, or listbox card control:

* Free text* Controlled by variable* Special value > User list or Group list

This method does not support add-in lists.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl7.html)

[IEdmCardControl7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018