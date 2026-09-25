<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~GetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVar Method (IEdmBomCell) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomCell Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html) : GetVar Method (IEdmBomCell) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVariableID*
:   ID of the variable to get (see **Remarks**)

*eColumn*
:   Type of column as defined in [EdmBomColumnType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html) (see **Remarks**)

*poValue*
:   Value in this BOM cell

*poComputedValue*
:   Computed value in this BOM cell

*pbsConfiguration*
:   Name of the configuration from which to get this BOM cell's value

*pbReadOnly*
:   True if this BOM cell cannot be updated, false if it can be updated by [IEdmBomCell::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~SetVar.html)

Gets the value of the specified cell in this BOM row.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetVar( _    ByVal lVariableID As System.Integer, _    ByVal eColumn As EdmBomColumnType, _    ByRef poValue As System.Object, _    ByRef poComputedValue As System.Object, _    ByRef pbsConfiguration As System.String, _    ByRef pbReadOnly As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVar(     System.int lVariableID,    EdmBomColumnType eColumn,    out System.object poValue,    out System.object poComputedValue,    out System.string pbsConfiguration,    out System.bool pbReadOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVar(  &   System.int lVariableID, &   EdmBomColumnType eColumn, &   [Out] System.Object^ poValue, &   [Out] System.Object^ poComputedValue, &   [Out] System.String^ pbsConfiguration, &   [Out] System.bool pbReadOnly ) ``` | |

#### Parameters

*lVariableID*
:   ID of the variable to get (see **Remarks**)

*eColumn*
:   Type of column as defined in [EdmBomColumnType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html) (see **Remarks**)

*poValue*
:   Value in this BOM cell

*poComputedValue*
:   Computed value in this BOM cell

*pbsConfiguration*
:   Name of the configuration from which to get this BOM cell's value

*pbReadOnly*
:   True if this BOM cell cannot be updated, false if it can be updated by [IEdmBomCell::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~SetVar.html)

# ![](dotnetimages/collapse.gif)Example

[Add Row to Bill of Materials (VB.NET)](Add_Row_to_Bill_of_Materials_Example_VBNET.htm)

[Add Row to Bill of Materials (C#)](Add_Row_to_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

1. Call [IEdmBomView::GetColumns](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView~GetColumns.html) to get [EdmBomColumn](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumn.html) for this BOM cell.- Set IVariableID with EdmBomColumn.mlVariableID.- Set eColumn with EdmBomColumn.meType.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomCell Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html)

[IEdmBomCell Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009