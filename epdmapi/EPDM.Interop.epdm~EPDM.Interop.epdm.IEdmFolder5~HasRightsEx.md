<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRightsEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| HasRightsEx Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : HasRightsEx Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lRights*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

*lFileID*
:   Optional ID of file on which to check lRights; 0 or null to check lRights on this folder only

Gets whether the user has the specified rights for the specified file in this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function HasRightsEx( _    ByVal lRights As System.Integer, _    Optional ByVal lFileID As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HasRightsEx(     System.int lRights,    System.int lFileID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool HasRightsEx(  &   System.int lRights, &   System.int lFileID ) ``` | |

#### Parameters

*lRights*
:   Combination of [EdmRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRightFlags.html) bits

*lFileID*
:   Optional ID of file on which to check lRights; 0 or null to check lRights on this folder only

#### Return Value

True if the user has all of the specified permissions, false if the user is missing one or more of the specified permissions

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method takes into account both the rights set explicitly on the user and those inherited from groups of which the user is a member. Optionally, you can specify the ID of a file for which to check rights. In that case, the rights-check includes workflow rights set on the current status of the file. If no file ID is specified, or it is 0, the rights-check is performed only on this folder.

**Note**: This method is only available in SOLIDWORKS PDM Professional Version 5.3 and later. If the program must have backward compatibility with SOLIDWORKS PDM Professional 5.2, use [IEdmFolder5::HasRights](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~HasRights.html) instead.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The user lacks one or more of the specified rights.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.3