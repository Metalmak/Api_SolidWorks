<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~GetNext.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNext Method (IEdmSelectionList5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html) : GetNext Method (IEdmSelectionList5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the item to get (see **Remarks**)

*pbsItemName*
:   Name of the file or folder (see **Remarks**)

*plItemID*
:   ID of the file or folder

*plParentFolderID*
:   ID of the parent folder of the file or folder

Obsolete. Superseded by [IEdmSelectionList6::GetNext2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~GetNext2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetNext( _    ByVal poPos As IEdmPos5, _    ByRef pbsItemName As System.String, _    ByRef plItemID As System.Integer, _    ByRef plParentFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetNext(     IEdmPos5 poPos,    out System.string pbsItemName,    out System.int plItemID,    out System.int plParentFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetNext(  &   IEdmPos5^ poPos, &   [Out] System.String^ pbsItemName, &   [Out] System.int plItemID, &   [Out] System.int plParentFolderID ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the item to get (see **Remarks**)

*pbsItemName*
:   Name of the file or folder (see **Remarks**)

*plItemID*
:   ID of the file or folder

*plParentFolderID*
:   ID of the parent folder of the file or folder

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first item, IEdmPos5. Call [IEdmSelectionList5::GetHeadPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~GetHeadPosition.html) to obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the items.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers must free the string returned in pbsItemName with a call to SysFreeString.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

[IEdmSelectionList5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2