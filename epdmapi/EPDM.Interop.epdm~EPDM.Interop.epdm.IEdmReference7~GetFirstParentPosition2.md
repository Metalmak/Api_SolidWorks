<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstParentPosition2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstParentPosition2 Method (IEdmReference7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html) : GetFirstParentPosition2 Method (IEdmReference7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersionOrZero*
:   Non-0 value enumerates the files referencing the specified version of the file; argument is ignored if value is 0

*bGetAllParentVersions*
:   True to return all versions, of all parents, referencing this file; false to return on the latest referencing version

*lEdmRefFlags*
:   Types of references that you want enumerated as defined in [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html)

Starts an enumeration of parent references.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstParentPosition2( _    ByVal lVersionOrZero As System.Integer, _    ByVal bGetAllParentVersions As System.Boolean, _    ByVal lEdmRefFlags As System.Integer _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstParentPosition2(     System.int lVersionOrZero,    System.bool bGetAllParentVersions,    System.int lEdmRefFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstParentPosition2(  &   System.int lVersionOrZero, &   System.bool bGetAllParentVersions, &   System.int lEdmRefFlags ) ``` | |

#### Parameters

*lVersionOrZero*
:   Non-0 value enumerates the files referencing the specified version of the file; argument is ignored if value is 0

*bGetAllParentVersions*
:   True to return all versions, of all parents, referencing this file; false to return on the latest referencing version

*lEdmRefFlags*
:   Types of references that you want enumerated as defined in [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html)

#### Return Value

[Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of first file referencing this file

# ![](dotnetimages/collapse.gif)Example

See the [IEdmReference7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Pass the position to [IEdmReference5::GetNextParent](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextParent.html) to continue to enumerate all of the parent files.

C++ programmers not using smart-pointer wrapper functions must release the position.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html)

[IEdmReference7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010