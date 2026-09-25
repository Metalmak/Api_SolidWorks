<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~SetHeader.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetHeader Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : SetHeader Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Header style as defined in swTableHeaderPosition\_e

*Count*
:   Number of lines in the header

Sets the header for this table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetHeader( _    ByVal Style As System.Integer, _    ByVal Count As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Style As System.Integer Dim Count As System.Integer Dim value As System.Boolean   value = instance.SetHeader(Style, Count) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetHeader(     System.int Style,    System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetHeader(  &   System.int Style, &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Header style as defined in swTableHeaderPosition\_e

*Count*
:   Number of lines in the header

#### Return Value

True if header is set successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::SetHeader.

# ![](dotnetimages/collapse.gif)Remarks

Tables created internally by the SOLIDWORKS software, such as Hole Charts, Revision Blocks, and BOM tables, are created with a specific number of headers lines.

This method cannot:

* Change the number of lines in the header for these tables; thus, the Count argument is ignored.* Turn off the header in these types of tables; thus, this method has no effect, and FALSE is returned.

Essentially, the only thing this method can do with these types of tables is to change the header between the top and the bottom.

If you are changing the header style and number of header lines in a single use of this method, the number of lines is considered before changing the header style. For example, if you are changing a table that had 1 header line at the top, by calling SetHeader (swTableHeader\_Bottom, 3), the first 3 lines in the table are moved to the bottom of the table.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::GetHeaderCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetHeaderCount.html)

[ITableAnnotation::GetHeaderStyle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetHeaderStyle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0