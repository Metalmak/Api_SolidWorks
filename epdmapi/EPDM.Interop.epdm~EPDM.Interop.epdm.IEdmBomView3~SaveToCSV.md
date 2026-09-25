<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView3~SaveToCSV.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SaveToCSV Method (IEdmBomView3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView3.html) : SaveToCSV Method (IEdmBomView3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFilePath*
:   Path and file name (**\*.CSV**) to which to save this BOM

*bCreateLevelColumn*
:   True to include a level column in the CSV file for an indented BOM, false to not

Saves this BOM to a comma separated values (CSV) file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SaveToCSV( _    ByVal bsFilePath As System.String, _    ByVal bCreateLevelColumn As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SaveToCSV(     System.string bsFilePath,    System.bool bCreateLevelColumn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SaveToCSV(  &   System.String^ bsFilePath, &   System.bool bCreateLevelColumn ) ``` | |

#### Parameters

*bsFilePath*
:   Path and file name (**\*.CSV**) to which to save this BOM

*bCreateLevelColumn*
:   True to include a level column in the CSV file for an indented BOM, false to not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomView3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView3.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomView3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView3.html)

[IEdmBomView3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017