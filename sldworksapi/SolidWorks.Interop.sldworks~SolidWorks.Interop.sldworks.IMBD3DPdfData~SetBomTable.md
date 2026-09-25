<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetBomTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBomTable Method (IMBD3DPdfData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMBD3DPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html) : SetBomTable Method (IMBD3DPdfData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of the BOM Table Area in the theme (see **Remarks**)

*BomTableName*
:   Name of the BOM table to map to the BOM Table Area specified by Index (see **Remarks**)

*Columns*
:   Array of strings of the names of the columns to export from the BOM table specified in BomTableName (see **Remarks**)

Maps a BOM Table Area in the [theme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) with a BOM table in the model and sets the columns in the BOM table to export to the BOM Table Area in a SOLIDWORKS MBD 3D PDF.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBomTable( _    ByVal Index As System.Integer, _    ByVal BomTableName As System.String, _    ByVal Columns As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMBD3DPdfData Dim Index As System.Integer Dim BomTableName As System.String Dim Columns As System.Object Dim value As System.Integer   value = instance.SetBomTable(Index, BomTableName, Columns) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetBomTable(     System.int Index,    System.string BomTableName,    System.object Columns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetBomTable(  &   System.int Index, &   System.String^ BomTableName, &   System.Object^ Columns ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of the BOM Table Area in the theme (see **Remarks**)

*BomTableName*
:   Name of the BOM table to map to the BOM Table Area specified by Index (see **Remarks**)

*Columns*
:   Array of strings of the names of the columns to export from the BOM table specified in BomTableName (see **Remarks**)

#### Return Value

0 = success; BOM table mapped

1 = failure; specified BomTableName not found in model

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MBD3DPdfData::SetBomTable.

# ![](dotnetimages/collapse.gif)Example

[Export BOM's Second Column to BOM Table Area (C#)](Export_BOM%27s_Second_Column_to_BOM_Table_Area_Example_CSharp.htm)

[Export BOM's Second Column to BOM Table Area (VB.NET)](Export_BOM%27s_Second_Column_to_BOM_Table_Area_Example_VBNET.htm)

[Export BOM's Second Column to BOM Table Area (VBA)](Export_BOM%27s_Second_Column_to_BOM_Table_Area_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| To get... | Call... |
| --- | --- |
| Index | [IMBD3PdfData::GetBomAreaCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetBomAreaCount.html) to find out the number of BOM Table Areas in the theme |
| BOMTableName | [IBomFeature::Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~Name.html) |
| Columns | * [ITableAnnotation::ColumnCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~ColumnCount.html) to get the number of columns in the BOM table* [ITableAnnotation::GetColumnTitle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetColumnTitle.html) for each column you want to export after getting the [table annotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) for the [BOM table annotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[IMBD3DPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html)

[IMBD3DPdfData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData_members.html)

[IMBD3DPdfData::ExcludeFromAnnotationView Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ExcludeFromAnnotationView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0