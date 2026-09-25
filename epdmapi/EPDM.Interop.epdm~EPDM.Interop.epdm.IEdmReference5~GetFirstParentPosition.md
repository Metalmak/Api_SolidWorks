<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetFirstParentPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstParentPosition Method (IEdmReference5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) : GetFirstParentPosition Method (IEdmReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersionOrZero*
:   Non-zero value enumerates the files referencing the specified version of the file; argument is ignored if value is 0

*bGetAllParentVersions*
:   True to return all versions, of all parents, referencing this file; false to return on the latest referencing version

Obsolete. Superseded by [IEdmReference7::GetFirstParentPosition2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstParentPosition2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstParentPosition( _    ByVal lVersionOrZero As System.Integer, _    ByVal bGetAllParentVersions As System.Boolean _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstParentPosition(     System.int lVersionOrZero,    System.bool bGetAllParentVersions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstParentPosition(  &   System.int lVersionOrZero, &   System.bool bGetAllParentVersions ) ``` | |

#### Parameters

*lVersionOrZero*
:   Non-zero value enumerates the files referencing the specified version of the file; argument is ignored if value is 0

*bGetAllParentVersions*
:   True to return all versions, of all parents, referencing this file; false to return on the latest referencing version

#### Return Value

[Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of first file referencing this file

# ![](dotnetimages/collapse.gif)Remarks

Pass the position to [IEdmReference6::GetNextParent](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextParent.html) to continue to enumerate all of the parent files.

C++ programmers not using smart-pointer wrapper functions must release the position.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional