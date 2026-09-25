<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20~GetTransitionCommentPermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetTransitionCommentPermissions Method (IEdmVault20) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault20 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20.html) : GetTransitionCommentPermissions Method (IEdmVault20) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lUserID*
:   User ID (see **Remarks**)

*poDocIds*
:   Array of document IDs (see **Remarks**)

*poTransNames*
:   Array of workfow transition names (see **Remarks**)

Gets whether the specified user must add a state change comment for the specified workflow transitions for the specified documents.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetTransitionCommentPermissions( _    ByVal lUserID As System.Integer, _    ByVal poDocIds() As System.Integer, _    ByVal poTransNames() As System.String _ ) As System.Boolean() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool[] GetTransitionCommentPermissions(     System.int lUserID,    System.int[] poDocIds,    System.string[] poTransNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.array<bool>^ GetTransitionCommentPermissions(  &   System.int lUserID, &   System.array<int>^ poDocIds, &   System.array<String^>^ poTransNames ) ``` | |

#### Parameters

*lUserID*
:   User ID (see **Remarks**)

*poDocIds*
:   Array of document IDs (see **Remarks**)

*poTransNames*
:   Array of workfow transition names (see **Remarks**)

#### Return Value

Array of booleans (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVault20](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The returned one-dimensional array contains (*n* \* *m*) booleans indicating whether lUserID must add a state change comment on each workflow transition in poTransNames for each document in poDocIds.

For:

* *n* = size of poDocIds* *m* = size of poTransNames* *permbool\_\** = true or false

the returned array follows the order of elements in poDocIds and poTransNames as follows:

{

*permbool\_poDocIds(0)\_poTransNames(0)*

*...*

*permbool\_poDocIds(0)\_poTransNames(m-1)*

*permbool\_poDocIds(1)\_poTransNames(0)*

*...*

*permbool\_poDocIds(1)\_poTransNames(m-1)*

*...*

*...*

*permbool\_poDocIds(n-1)\_poTransNames(0)*

*...*

*permbool\_poDocIds(n-1)\_poTransNames(m-1)*

}

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault20 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20.html)

[IEdmVault20 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019