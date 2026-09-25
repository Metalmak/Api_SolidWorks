<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstChildPosition2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstChildPosition2 Method (IEdmReference7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html) : GetFirstChildPosition2 Method (IEdmReference7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*pbsProjectName*
:   Project name (see **Remarks**)

*bIsTopParent*
:   True if this is the topmost node in the reference tree, false if not

*bPermitReadLocal*
:   True to allow SOLIDWORKS PDM Professional to read reference information if it is not already present in the database, false to disallow SOLIDWORKS PDM Professional to read reference information if it is not already present in the database

*lEdmRefFlags*
:   Types of references that you want enumerated as defined in [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html)

*lVersion*
:   Version for which to get references; use 0 for latest version

Obsolete. Superseded by [IEdmReference9::GetFirstChildPosition3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference9~GetFirstChildPosition3.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstChildPosition2( _    ByRef pbsProjectName As System.String, _    ByVal bIsTopParent As System.Boolean, _    ByVal bPermitReadLocal As System.Boolean, _    ByVal lEdmRefFlags As System.Integer, _    Optional ByVal lVersion As System.Integer _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstChildPosition2(     out System.string pbsProjectName,    System.bool bIsTopParent,    System.bool bPermitReadLocal,    System.int lEdmRefFlags,    System.int lVersion ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstChildPosition2(  &   [Out] System.String^ pbsProjectName, &   System.bool bIsTopParent, &   System.bool bPermitReadLocal, &   System.int lEdmRefFlags, &   System.int lVersion ) ``` | |

#### Parameters

*pbsProjectName*
:   Project name (see **Remarks**)

*bIsTopParent*
:   True if this is the topmost node in the reference tree, false if not

*bPermitReadLocal*
:   True to allow SOLIDWORKS PDM Professional to read reference information if it is not already present in the database, false to disallow SOLIDWORKS PDM Professional to read reference information if it is not already present in the database

*lEdmRefFlags*
:   Types of references that you want enumerated as defined in [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html)

*lVersion*
:   Version for which to get references; use 0 for latest version

#### Return Value

[Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of the first file referenced by this file (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

You should maintain and pass in a string, by reference, in this argument for all calls to this method in a reference tree. The project name can be allocated and returned by the topmost node in the tree and is used by its children.

Pass the position returned by this method to [IEdmReference5::GetNextChild](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextChild.html) to continue to enumerate the referenced files.

C++ programmers not using smart-pointer wrapper functions must release the position.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html)

[IEdmReference7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010