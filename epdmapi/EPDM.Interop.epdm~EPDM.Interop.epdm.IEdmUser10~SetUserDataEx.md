<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetUserDataEx Method (IEdmUser10) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html) : SetUserDataEx Method (IEdmUser10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poUserData*
:   [EdmUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) structure (see **Remarks**)

Sets information about this user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetUserDataEx( _    ByRef poUserData As EdmUserDataEx _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetUserDataEx(     ref EdmUserDataEx poUserData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetUserDataEx(  &   EdmUserDataEx% poUserData ) ``` | |

#### Parameters

*poUserData*
:   [EdmUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) structure (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUser10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The properties and picture associated with this user can be updated using this method. EdmUserDataEx::mlEdmUserDataExFlags indicates which properties to update. EdmUserDataEx::mlUserID is ignored.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user doesn't have user administration privileges.* E\_EDM\_FILE\_NOT\_FOUND: A new user picture path was specified, but the file wasn't found.* E\_EDM\_INVALID\_FILE: A new user picture path was specified, but the file format isn't supported.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html)

[IEdmUser10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013