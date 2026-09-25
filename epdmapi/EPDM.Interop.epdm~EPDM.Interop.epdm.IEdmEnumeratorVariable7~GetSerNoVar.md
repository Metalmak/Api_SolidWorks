<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7~GetSerNoVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSerNoVar Method (IEdmEnumeratorVariable7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html) : GetSerNoVar Method (IEdmEnumeratorVariable7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSerNoName*
:   Serial number of variables to find

*lFolderID*
:   ID of the file's parent folder; 0 if the file is not shared

*ppoRetIDs*
:   Array of IDs of variables with bSerNoName

Gets the IDs of all variables that have the specified serial number.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetSerNoVar( _    ByVal bsSerNoName As System.String, _    ByVal lFolderID As System.Integer, _    ByRef ppoRetIDs() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSerNoVar(     System.string bsSerNoName,    System.int lFolderID,    out System.int[] ppoRetIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSerNoVar(  &   System.String^ bsSerNoName, &   System.int lFolderID, &   [Out] System.array<int>^ ppoRetIDs ) ``` | |

#### Parameters

*bsSerNoName*
:   Serial number of variables to find

*lFolderID*
:   ID of the file's parent folder; 0 if the file is not shared

*ppoRetIDs*
:   Array of IDs of variables with bSerNoName

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7.html)

[IEdmEnumeratorVariable7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4