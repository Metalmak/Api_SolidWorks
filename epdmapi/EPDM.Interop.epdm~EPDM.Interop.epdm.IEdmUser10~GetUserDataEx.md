<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~GetUserDataEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetUserDataEx Method (IEdmUser10) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUser10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html) : GetUserDataEx Method (IEdmUser10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poUserData*
:   [EdmUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) (see **Remarks**)

Gets information about this user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetUserDataEx( _    ByRef poUserData As EdmUserDataEx _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetUserDataEx(     out EdmUserDataEx poUserData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetUserDataEx(  &   [Out] EdmUserDataEx poUserData ) ``` | |

#### Parameters

*poUserData*
:   [EdmUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUser10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The properties and picture associated with this user can be returned. EdmUserDataEx::mlEdmUserDataExFlags indicates which properties to return.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUser10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10.html)

[IEdmUser10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10_members.html)

[IEdmuser10::SetUserDataEx Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013