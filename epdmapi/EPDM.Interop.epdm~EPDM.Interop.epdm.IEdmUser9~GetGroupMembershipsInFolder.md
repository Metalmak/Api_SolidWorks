<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser9~GetGroupMembershipsInFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetGroupMembershipsInFolder Method (IEdmUser9) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser9.html) : GetGroupMembershipsInFolder Method (IEdmUser9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of folder for which to get memberships

Gets all of the groups to which this user belongs and for the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetGroupMembershipsInFolder( _    ByVal lFolderID As System.Integer _ ) As System.Object() ``` | |

| C# |  |
| --- | --- |
| ``` System.object[] GetGroupMembershipsInFolder(     System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.array<Object^>^ GetGroupMembershipsInFolder(  &   System.int lFolderID ) ``` | |

#### Parameters

*lFolderID*
:   ID of folder for which to get memberships

#### Return Value

Array of [IEdmUserGroup8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup8.html) interfaces

# ![](dotnetimages/collapse.gif)Example

[Add and Remove User and Group from Folder (C#)](Add_and_Remove_User_and_Group_from_Folder_Example_CSharp.htm)

[Add and Remove User and Group from Folder (VB.NET)](Add_and_Remove_User_and_Group_from_Folder_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method extends [IEdmUser8::GetGroupMemberships](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser8~GetGroupMemberships.html), which only gets global group memberships. As of SOLIDWORKS PDM Professional 2011, it is possible to assign group memberships to a specific folder. This method gets folder-specific group memberships.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser9.html)

[IEdmUser9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011