<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6~AddReference2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddReference2 Method (IEdmEnumeratorCustomReference6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorCustomReference6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6.html) : AddReference2 Method (IEdmEnumeratorCustomReference6) |

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

*lQuantity*
:   Number of times the referenced file is referenced

Obsolete. Superseded by [IEdmEnumeratorCustomReference7::AddReference3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~AddReference3.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddReference2( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer, _    ByVal lQuantity As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddReference2(     System.int lFileID,    System.int lFolderID,    System.int lQuantity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddReference2(  &   System.int lFileID, &   System.int lFolderID, &   System.int lQuantity ) ``` | |

#### Parameters

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

*lQuantity*
:   Number of times the referenced file is referenced

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: File is not checked out.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6.html)

[IEdmEnumeratorCustomReference6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013