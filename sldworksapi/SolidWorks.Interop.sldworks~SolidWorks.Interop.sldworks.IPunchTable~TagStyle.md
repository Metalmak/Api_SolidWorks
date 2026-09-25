<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable~TagStyle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| TagStyle Property (IPunchTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html) : TagStyle Property (IPunchTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the tag style for this punch table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property TagStyle As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPunchTable Dim value As System.Integer   instance.TagStyle = value   value = instance.TagStyle ``` | |

| C# |  |
| --- | --- |
| ``` System.int TagStyle {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int TagStyle {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Tag style as defined by swPunchTableTagStyle\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PunchTable::TagStyle.

# ![](dotnetimages/collapse.gif)Example

[Insert Punch Table (VBA)](Insert_Punch_Table_Example_VB.htm)

[Insert Punch Table (VB.NET)](Insert_Punch_Table_Example_VBNET.htm)

[Insert Punch Table (C#)](Insert_Punch_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html)

[IPunchTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable_members.html)

[IPunch::CombineTags Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable~CombineTags.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0