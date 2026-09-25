<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~AddReferencesPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddReferencesPath Method (IEdmAddCustomRefs) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html) : AddReferencesPath Method (IEdmAddCustomRefs) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lRootFile*
:   ID of file to which to add file references

*ppoReferences*
:   Array of paths to reference files to add to lRootFile

Obsolete. Superseded by [IEdmAddCustomRefs2::AddReferencesPath2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2~AddReferencesPath2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddReferencesPath( _    ByVal lRootFile As System.Integer, _    ByRef ppoReferences() As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddReferencesPath(     System.int lRootFile,    ref System.string[] ppoReferences ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddReferencesPath(  &   System.int lRootFile, &   System.array<String^>^% ppoReferences ) ``` | |

#### Parameters

*lRootFile*
:   ID of file to which to add file references

*ppoReferences*
:   Array of paths to reference files to add to lRootFile

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html)

[IEdmAddCustomRefs Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional