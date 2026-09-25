<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable~GetTableAnnotations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTableAnnotations Method (IPunchTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html) : GetTableAnnotations Method (IPunchTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the punch table annotations for this punch table feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTableAnnotations() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPunchTable Dim value As System.Object   value = instance.GetTableAnnotations() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetTableAnnotations() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetTableAnnotations(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [IPunchTableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPunchTableAnnotation.html) objects for this punch table feature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PunchTable::GetTableAnnotations.

# ![](dotnetimages/collapse.gif)Example

[Insert Punch Table (VBA)](Insert_Punch_Table_Example_VB.htm)

[Insert Punch Table (VB.NET)](Insert_Punch_Table_Example_VBNET.htm)

[Insert Punch Table (C#)](Insert_Punch_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method gets all of the table annotations of a split table. Many of the [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html) methods and properties get table annotation information that is common to all table annotations. You should apply these [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html) methods and properties to only one of the split table annotations returned by this method. Otherwise, you will get redundant data.

# ![](dotnetimages/collapse.gif)See Also

####

[IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html)

[IPunchTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable_members.html)

[IPunchTable::IGetTableAnnotations Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable~IGetTableAnnotations.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0