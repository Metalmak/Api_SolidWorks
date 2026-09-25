<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3~VerUpgrade_ReferenceCheck.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| VerUpgrade\_ReferenceCheck Method (IEdmRevisionMgr3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3.html) : VerUpgrade\_ReferenceCheck Method (IEdmRevisionMgr3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poFiles*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures; one structure for each assembly file for which to find references

*ppoWrongRefs*
:   Array of [EdmCheckRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef.html) structures; one structure for each part that is referenced in an earlier version than the lastest version

Finds parts that are referenced by assemblies and where the referenced part version is not the latest version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub VerUpgrade_ReferenceCheck( _    ByVal poFiles() As EdmSelItem, _    ByRef ppoWrongRefs() As EdmCheckRef _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void VerUpgrade_ReferenceCheck(     EdmSelItem[] poFiles,    out EdmCheckRef[] ppoWrongRefs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void VerUpgrade_ReferenceCheck(  &   array<EdmSelItem>^ poFiles, &   [Out] array<EdmCheckRef>^ ppoWrongRefs ) ``` | |

#### Parameters

*poFiles*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures; one structure for each assembly file for which to find references

*ppoWrongRefs*
:   Array of [EdmCheckRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCheckRef.html) structures; one structure for each part that is referenced in an earlier version than the lastest version

# ![](dotnetimages/collapse.gif)Remarks

You need to be logged in as a user that has permission to update revision numbers ([EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html).EdmSysRight\_ModifyRevisionNumbers) in order to use this method. The reason you need this high level of permission is that this method overrides read permission on the files and returns files that the logged-in user lacks permission to see.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3.html)

[IEdmRevisionMgr3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009