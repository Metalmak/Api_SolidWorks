<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3~GetReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetReferences Method (IEdmBatchListing3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3.html) : GetReferences Method (IEdmBatchListing3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoReferences*
:   Array of [EdmListRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRef.html) structures

Gets a list of referenced files.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetReferences( _    ByRef ppoReferences() As EdmListRef _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReferences(     out EdmListRef[] ppoReferences ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReferences(  &   [Out] array<EdmListRef>^ ppoReferences ) ``` | |

#### Parameters

*ppoReferences*
:   Array of [EdmListRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRef.html) structures

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3.html)

[IEdmBatchListing3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010