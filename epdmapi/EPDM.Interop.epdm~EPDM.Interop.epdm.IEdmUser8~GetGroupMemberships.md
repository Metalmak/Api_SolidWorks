<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser8~GetGroupMemberships.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetGroupMemberships Method (IEdmUser8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser8.html) : GetGroupMemberships Method (IEdmUser8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poGroups*
:   Array of [IEdmUserGroup6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html) interfaces

Gets all of the groups to which this user belongs.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetGroupMemberships( _    ByRef poGroups() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetGroupMemberships(     out System.object[] poGroups ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetGroupMemberships(  &   [Out] System.array<Object^>^ poGroups ) ``` | |

#### Parameters

*poGroups*
:   Array of [IEdmUserGroup6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup6.html) interfaces

# ![](dotnetimages/collapse.gif)Example

The following sample code displays a message box with the names of all the groups to which a user, John, belongs:

Private Sub GetJohnsGroups(ByVal vault As IEdmVault12)

  'Get the user interface of user 'John'
  Dim userMgr As IEdmUserMgr7
  userMgr = vault.CreateUtility(EdmUtility.EdmUtil\_UserMgr)
  Dim john As IEdmUser8
  john = userMgr.GetUser("John")

  'Get the groups to which he belongs
  Dim groups() As Object
  groups = Nothing
  john.GetGroupMemberships(groups)

  'Display a message box with the group names
  Dim message As String
  message = "John's groups:" + vbLf
  Dim i As Integer
  i = LBound(groups)
  While (i <= UBound(groups))
    Dim group As IEdmUserGroup7
    group = groups(i)
    message = message + group.Name + vbLf
    i = i + 1
  End While

  MsgBox(message)

End Sub

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser8.html)

[IEdmUser8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser8_members.html)

[IEdmUser9::GetGroupMembershipsInFolder Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser9~GetGroupMembershipsInFolder.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011