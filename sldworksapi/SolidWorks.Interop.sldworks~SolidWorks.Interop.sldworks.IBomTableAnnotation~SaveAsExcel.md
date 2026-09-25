<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~SaveAsExcel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveAsExcel Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : SaveAsExcel Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path and file name of the Microsoft Excel file to save to (**\*.xls**)

*IncludeHidden*
:   True to include text in hidden cells, false to not

*IncludeFileImages*
:   True to include file images, false to not

Saves this BOM table annotation as a Microsoft Excel document with the specified properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveAsExcel( _    ByVal FileName As System.String, _    ByVal IncludeHidden As System.Boolean, _    ByVal IncludeFileImages As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim FileName As System.String Dim IncludeHidden As System.Boolean Dim IncludeFileImages As System.Boolean Dim value As System.Boolean   value = instance.SaveAsExcel(FileName, IncludeHidden, IncludeFileImages) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveAsExcel(     System.string FileName,    System.bool IncludeHidden,    System.bool IncludeFileImages ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveAsExcel(  &   System.String^ FileName, &   System.bool IncludeHidden, &   System.bool IncludeFileImages ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path and file name of the Microsoft Excel file to save to (**\*.xls**)

*IncludeHidden*
:   True to include text in hidden cells, false to not

*IncludeFileImages*
:   True to include file images, false to not

#### Return Value

True if the table is saved as a Microsoft Excel file, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::SaveAsExcel.

# ![](dotnetimages/collapse.gif)Example

[Save Table to Microsoft Excel (VBA)](Save_Table_to_Microsoft_Excel_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0