<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~HoleTag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| HoleTag Property (IHoleTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html) : HoleTag Property (IHoleTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Row*
:   0-based index of the row in which you want to change the name of the tag

Gets or sets the name of the specified tag in a hole table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property HoleTag( _    ByVal Row As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleTable Dim Row As System.Integer Dim value As System.String   instance.HoleTag(Row) = value   value = instance.HoleTag(Row) ``` | |

| C# |  |
| --- | --- |
| ``` System.string HoleTag(     System.int Row ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ HoleTag {    System.String^ get(System.int Row);    void set (System.int Row, System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Row*
:   0-based index of the row in which you want to change the name of the tag

#### Property Value

Tag name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleTable::HoleTag.

# ![](dotnetimages/collapse.gif)Example

[Change Tags in Hole Table (VB.NET)](Change_Tags_in_Hole_Table_Example_VBNET.htm)

[Change Tags in Hole Table (VBA)](Change_Tags_in_Hole_Table_Example_VB.htm)

[Change Tags in Hole Table (C#)](Change_Tags_in_Hole_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[IHoleTable::CombineTags](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IHoleTable~CombineTags.html) must be false for IHoleTable::HoleTag to work.

If you plan on changing many hole tags, then consider setting [IHoleTable::EnableUpdate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IHoleTable~EnableUpdate.html) to false to avoid a possible degradation in performance. After changing all of the hole tags, set IHoleTable::EnableUpdate to true to update the hole table and model view.

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html)

[IHoleTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable_members.html)

[IHoleTable::HoleTagsVisible Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~HoleTagsVisible.html)

[IHoleTable::TagStyle Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~TagStyle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0