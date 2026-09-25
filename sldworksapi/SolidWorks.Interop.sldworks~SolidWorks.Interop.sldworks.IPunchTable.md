<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPunchTable Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPunchTable Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to punch table information and values.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPunchTable ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPunchTable ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPunchTable ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPunchTable ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PunchTable.

# ![](dotnetimages/collapse.gif)Example

[Insert Punch Table (C#)](Insert_Punch_Table_Example_CSharp.htm)

[Insert Punch Table (VB.NET)](Insert_Punch_Table_Example_VBNET.htm)

[Insert Punch Table (VBA)](Insert_Punch_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Punch tables contain information about the punches that are created by forming tools in sheet metal parts. A punch table contains the following information about pre-selected punches:

| Column | Description |
| --- | --- |
| TAG | Datum tag added to each punch in the flat pattern view |
| PUNCH ID | Property of the forming tool or library feature |
| X Location | Distance from the x-axis to the point of insertion of the forming tool in the flat pattern view |
| Y Location | Distance from the y-axis to the point of insertion of the forming tool in the flat pattern view |
| ANGLE | Angle between the x-axis and the forming tool |
| QUANTITY | Number of times that the forming tool is used in the flat pattern view |

# ![](dotnetimages/collapse.gif)Accessors

[IPunchTableAnnotation::PunchTable](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPunchTableAnnotation~PunchTable.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[PunchTable](SWObjectModel.pdf#PunchTable)

# ![](dotnetimages/collapse.gif)See Also

####

[IPunchTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IPunchTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTableAnnotation.html)

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)