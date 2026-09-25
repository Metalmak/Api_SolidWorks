<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~SetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetVar Method (IEdmBomCell) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomCell Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html) : SetVar Method (IEdmBomCell) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVariableID*
:   ID of the variable to set (see **Remarks**)

*eColumn*
:   Type of column as defined in [EdmBomColumnType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html) (see **Remarks**)

*oNewValue*
:   New value

*bsConfiguration*
:   Name of the configuration in which to set the value of this BOM cell

*eOption*
:   Type of value to set as defined in [EdmBomSetVarOption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomSetVarOption.html)

*pbsErrorMessage*
:   Error message

Sets the value of the specified cell in this BOM row.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function SetVar( _    ByVal lVariableID As System.Integer, _    ByVal eColumn As EdmBomColumnType, _    ByVal oNewValue As System.Object, _    ByVal bsConfiguration As System.String, _    ByVal eOption As EdmBomSetVarOption, _    ByRef pbsErrorMessage As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetVar(     System.int lVariableID,    EdmBomColumnType eColumn,    System.object oNewValue,    System.string bsConfiguration,    EdmBomSetVarOption eOption,    out System.string pbsErrorMessage ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetVar(  &   System.int lVariableID, &   EdmBomColumnType eColumn, &   System.Object^ oNewValue, &   System.String^ bsConfiguration, &   EdmBomSetVarOption eOption, &   [Out] System.String^ pbsErrorMessage ) ``` | |

#### Parameters

*lVariableID*
:   ID of the variable to set (see **Remarks**)

*eColumn*
:   Type of column as defined in [EdmBomColumnType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomColumnType.html) (see **Remarks**)

*oNewValue*
:   New value

*bsConfiguration*
:   Name of the configuration in which to set the value of this BOM cell

*eOption*
:   Type of value to set as defined in [EdmBomSetVarOption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomSetVarOption.html)

*pbsErrorMessage*
:   Error message

#### Return Value

True if the value is successfully set, false if not

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