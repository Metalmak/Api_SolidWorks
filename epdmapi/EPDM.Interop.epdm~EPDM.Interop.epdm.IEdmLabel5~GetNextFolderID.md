<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5~GetNextFolderID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextFolderID Method (IEdmLabel5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmLabel5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html) : GetNextFolderID Method (IEdmLabel5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next folder (see **Remarks**)

Gets the next ID of a folder with this label in the enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextFolderID( _    ByVal poPos As IEdmPos5 _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetNextFolderID(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetNextFolderID(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next folder (see **Remarks**)

#### Return Value

ID of folder on which this label is set

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first folder with this label, IEdmPos5. Call [IEdmLabel5::GetFirstFolderPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5~GetFirstFolderPosition.html) to obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the folder IDs.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmLabel5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html)

[IEdmLabel5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2