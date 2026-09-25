<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~InsertColumn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertColumn Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : InsertColumn Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Where*
:   Where to insert the column as specified in swTableItemInsertPosition\_e

*Index*
:   Index of the column where to insert the new column

*Name*
:   Column name

Obsolete. Superseded by [ITableAnnnotation::InsertColumn2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~InsertColumn2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertColumn( _    ByVal Where As System.Integer, _    ByVal Index As System.Integer, _    ByVal Name As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Where As System.Integer Dim Index As System.Integer Dim Name As System.String Dim value As System.Boolean   value = instance.InsertColumn(Where, Index, Name) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertColumn(     System.int Where,    System.int Index,    System.string Name ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertColumn(  &   System.int Where, &   System.int Index, &   System.String^ Name ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Where*
:   Where to insert the column as specified in swTableItemInsertPosition\_e

*Index*
:   Index of the column where to insert the new column

*Name*
:   Column name

#### Return Value

True if column is inserted successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::InsertColumn.

# ![](dotnetimages/collapse.gif)Example

[Insert Part Number Column in BOM Table (C#)](Insert_Part_Number_Column_in_BOM_Table_Example_CSharp.htm)

[Insert Part Number Column in BOM Table (VB.NET)](Insert_Part_Number_Column_in_BOM_Table_Example_VBNET.htm)

[Insert Part Number Column in BOM Table (VBA)](Insert_Part_Number_Column_in_BOM_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The index for both rows and columns is 0-based.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0