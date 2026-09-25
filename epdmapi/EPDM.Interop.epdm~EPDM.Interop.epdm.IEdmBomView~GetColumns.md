<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView~GetColumns.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetColumns Method (IEdmBomView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html) : GetColumns Method (IEdmBomView) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoColumns*
:   Array of [EdmBomColumn](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn.html) structures; one structure for each BOM column

Gets the column definitions for this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetColumns( _    ByRef ppoColumns() As EdmBomColumn _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetColumns(     out EdmBomColumn[] ppoColumns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetColumns(  &   [Out] array<EdmBomColumn>^ ppoColumns ) ``` | |

#### Parameters

*ppoColumns*
:   Array of [EdmBomColumn](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn.html) structures; one structure for each BOM column

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