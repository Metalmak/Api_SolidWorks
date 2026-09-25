<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~AddTail.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddTail Method (IEdmSelectionList5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html) : AddTail Method (IEdmSelectionList5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsItemName*
:   File or folder name

*lItemID*
:   ID of file or folder

*lParentFolderID*
:   ID of parent folder of file or folder

Obsolete. Superseded by [IEdmSelectionList6::AddTail2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~AddTail2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddTail( _    ByVal bsItemName As System.String, _    ByVal lItemID As System.Integer, _    ByVal lParentFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddTail(     System.string bsItemName,    System.int lItemID,    System.int lParentFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddTail(  &   System.String^ bsItemName, &   System.int lItemID, &   System.int lParentFolderID ) ``` | |

#### Parameters

*bsItemName*
:   File or folder name

*lItemID*
:   ID of file or folder

*lParentFolderID*
:   ID of parent folder of file or folder

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

[IEdmSelectionList5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2