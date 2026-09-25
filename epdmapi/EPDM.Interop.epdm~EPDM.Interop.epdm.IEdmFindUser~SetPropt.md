<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SetPropt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetPropt Method (IEdmFindUser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) : SetPropt Method (IEdmFindUser) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eProp*
:   User property to search for as defined by [EdmFindUserProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFindUserProp.html)

*oValue*
:   Value of the property specified in eProp

Sets the search criteria for finding users.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetPropt( _    ByVal eProp As EdmFindUserProp, _    ByVal oValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPropt(     EdmFindUserProp eProp,    System.object oValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPropt(  &   EdmFindUserProp eProp, &   System.Object^ oValue ) ``` | |

#### Parameters

*eProp*
:   User property to search for as defined by [EdmFindUserProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFindUserProp.html)

*oValue*
:   Value of the property specified in eProp

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call one of the following:

* [IEdmFindUser::SilentFind](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SilentFind.html) to silently search for users matching the criteria specified by this method.* [IEdmFindUser::ShowFindUI](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~ShowFindUI.html) to display a search user interface that is populated with the criteria specified by this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html)

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013