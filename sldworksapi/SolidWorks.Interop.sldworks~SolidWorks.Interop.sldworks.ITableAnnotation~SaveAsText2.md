<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SaveAsText2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveAsText2 Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : SaveAsText2 Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path and filename of text data file (see **Remarks**)

*Separator*
:   Character or string to use to separate each of the text within each of the cells in the table in the text file (see **Remarks**)

*IncludeHidden*
:   True to include text in hidden cells, false to not

Saves this table to a text data file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveAsText2( _    ByVal FileName As System.String, _    ByVal Separator As System.String, _    ByVal IncludeHidden As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim FileName As System.String Dim Separator As System.String Dim IncludeHidden As System.Boolean Dim value As System.Boolean   value = instance.SaveAsText2(FileName, Separator, IncludeHidden) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveAsText2(     System.string FileName,    System.string Separator,    System.bool IncludeHidden ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveAsText2(  &   System.String^ FileName, &   System.String^ Separator, &   System.bool IncludeHidden ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path and filename of text data file (see **Remarks**)

*Separator*
:   Character or string to use to separate each of the text within each of the cells in the table in the text file (see **Remarks**)

*IncludeHidden*
:   True to include text in hidden cells, false to not

#### Return Value

True if table is saved as a text file, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::SaveAsText2.

# ![](dotnetimages/collapse.gif)Remarks

FileName should include the path, filename, and filename extension to which to save the table as a text file.

|  |  |
| --- | --- |
| **If a file of the specified name in the specified path...** | **Then it is...** |
| Exists | Overwritten |
| Does not exist | Created |

Separator is typically a single character, but it can be a string. If Separator is empty, then the tab character is used.

**NOTE**: Although you can save a table as a text file for use with other applications, like Microsoft Excel, you cannot currently import a text file to a table in SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::SaveAsPDF Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SaveAsPDF.html)

[ITableAnnotation::SaveAsTemplate Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SaveAsTemplate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0