<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView~GetRows.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRows Method (IEdmBomView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html) : GetRows Method (IEdmBomView) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRows*
:   Array of [IEdmBomCells](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html); one interface for each BOM row

Gets the row definitions for this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRows( _    ByRef ppoRows() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRows(     out System.object[] ppoRows ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRows(  &   [Out] System.array<Object^>^ ppoRows ) ``` | |

#### Parameters

*ppoRows*
:   Array of [IEdmBomCells](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html); one interface for each BOM row

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomView Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html)

[IEdmBomView Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009