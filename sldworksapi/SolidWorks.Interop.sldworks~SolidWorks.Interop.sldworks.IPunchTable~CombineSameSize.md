<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable~CombineSameSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CombineSameSize Property (IPunchTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html) : CombineSameSize Property (IPunchTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to merge Punch ID column cells that have the same contents.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CombineSameSize As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPunchTable Dim value As System.Boolean   instance.CombineSameSize = value   value = instance.CombineSameSize ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CombineSameSize {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool CombineSameSize {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to merge Punch ID column cells that have the same contents, false to not; only valid if [IPunchTable::CombineTags](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPunchTable~CombineTags.html) is false (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PunchTable::CombineSameSize.

# ![](dotnetimages/collapse.gif)Example

[Insert Punch Table (C#)](Insert_Punch_Table_Example_CSharp.htm)

[Insert Punch Table (VB.NET)](Insert_Punch_Table_Example_VBNET.htm)

[Insert Punch Table (VBA)](Insert_Punch_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Set this property to true to create a punch table with a PUNCH ID column that contains column cells that have been merged because they contain the same value within each tag group (e.g., A1, A2, A3).

If this property is set to false, the punch table looks like this:

| TAG | PUNCH ID | X LOCATION | Y LOCATION | ANGLE | QUANTITY |
| --- | --- | --- | --- | --- | --- |
| A1 | 135 | 107 | 300 | 90 | 1 |
| A2 | 135 | 200 | 150 | 90 | 1 |
| A3 | 135 | 300 | 200 | 90 | 1 |

If this property is set to true, the punch table looks like this:

| TAG | PUNCH ID | X LOCATION | Y LOCATION | ANGLE | QUANTITY |
| --- | --- | --- | --- | --- | --- |
| A1 | 135 | 107 | 300 | 90 | 1 |
| A2 | 200 | 150 | 90 | 1 |
| A3 | 300 | 200 | 90 | 1 |

# ![](dotnetimages/collapse.gif)See Also

####

[IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html)

[IPunchTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0