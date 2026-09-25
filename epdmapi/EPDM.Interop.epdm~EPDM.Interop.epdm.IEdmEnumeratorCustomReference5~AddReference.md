<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5~AddReference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddReference Method (IEdmEnumeratorCustomReference5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorCustomReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5.html) : AddReference Method (IEdmEnumeratorCustomReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

Obsolete. Superseded by [IEdmEnumeratorCustomReference6::AddReference2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6~AddReference2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddReference( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddReference(     System.int lFileID,    System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddReference(  &   System.int lFileID, &   System.int lFolderID ) ``` | |

#### Parameters

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: File is not checked out.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5.html)

[IEdmEnumeratorCustomReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2