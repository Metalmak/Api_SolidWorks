<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetSplitInformation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSplitInformation Method (ITableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : GetSplitInformation Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Piece of the table that this is

*Count*
:   Piece of the table that this is

*RangeStart*
:   Beginning row for this piece of the table

*RangeEnd*
:   Ending row for this piece of the table

Gets information about any splits in this table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSplitInformation( _    ByRef Index As System.Integer, _    ByRef Count As System.Integer, _    ByRef RangeStart As System.Integer, _    ByRef RangeEnd As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim Index As System.Integer Dim Count As System.Integer Dim RangeStart As System.Integer Dim RangeEnd As System.Integer Dim value As System.Integer   value = instance.GetSplitInformation(Index, Count, RangeStart, RangeEnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSplitInformation(     out System.int Index,    out System.int Count,    out System.int RangeStart,    out System.int RangeEnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSplitInformation(  &   [Out] System.int Index, &   [Out] System.int Count, &   [Out] System.int RangeStart, &   [Out] System.int RangeEnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Piece of the table that this is

*Count*
:   Piece of the table that this is

*RangeStart*
:   Beginning row for this piece of the table

*RangeEnd*
:   Ending row for this piece of the table

#### Return Value

Direction in which the table was split as defined by swTableSplitDirection\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::GetSplitInformation.

# ![](dotnetimages/collapse.gif)Example

[Export BOMs to XML (C#)](Export_BOMs_to_XML_Example_CSharp.htm)

[Export BOMs to XML (VB.NET)](Export_BOMs_to_XML_Example_VBNET.htm)

[Export BOMs to XML (VBA)](Export_BOMs_to_XML_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A table split is a table divided into multiple tables, also called pieces.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::Split Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~Split.html)

[ITableAnnotation::HorizontalAutoSplit Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~HorizontalAutoSplit.html)

[ITableAnnotation::StopAutoSplitting Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~StopAutoSplitting.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0