<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7~Rollback3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback3 Method (IEdmRevision7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevision7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7.html) : Rollback3 Method (IEdmRevision7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment for this revision

*vbRedirectParentRefs*
:   True to roll back the file with its parent references, false to roll back the file without its parent references

Rolls this file back to the version of this revision.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback3( _    ByVal bsComment As System.String, _    ByVal vbRedirectParentRefs As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback3(     System.string bsComment,    System.bool vbRedirectParentRefs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback3(  &   System.String^ bsComment, &   System.bool vbRedirectParentRefs ) ``` | |

#### Parameters

*bsComment*
:   Comment for this revision

*vbRedirectParentRefs*
:   True to roll back the file with its parent references, false to roll back the file without its parent references

# ![](dotnetimages/collapse.gif)Example

[Roll Back Revisions (C#)](Roll_Back_Revisions_Example_CSharp.htm)

[Roll Back Revisions (VB.NET)](Roll_Back_Revisions_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after this revision number. To undo this rollback operation, you need to restore a backup of the entire database and file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevision7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7.html)

[IEdmRevision7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7_members.html)

[IEdmEnumeratorVersion7::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7~Rollback3.html)

[IEdmVersion8::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8~Rollback3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017