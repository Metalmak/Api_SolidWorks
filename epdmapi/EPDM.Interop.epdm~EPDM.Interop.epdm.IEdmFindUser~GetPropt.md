<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~GetPropt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetPropt Method (IEdmFindUser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) : GetPropt Method (IEdmFindUser) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eProp*
:   User property to search for as defined by [EdmFindUserProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFindUserProp.html)

Gets the search criteria previously set by [IEdmFindUser::SetPropt](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SetPropt.html) for finding users.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetPropt( _    ByVal eProp As EdmFindUserProp _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPropt(     EdmFindUserProp eProp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPropt(  &   EdmFindUserProp eProp ) ``` | |

#### Parameters

*eProp*
:   User property to search for as defined by [EdmFindUserProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFindUserProp.html)

#### Return Value

Value of the property specified in eProp

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html)

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013