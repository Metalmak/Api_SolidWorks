<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark~GroupCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GroupCount Property (ICenterMark) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html) : GroupCount Property (ICenterMark) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of center marks in a center mark set.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property GroupCount As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICenterMark Dim value As System.Integer   value = instance.GroupCount ``` | |

| C# |  |
| --- | --- |
| ``` System.int GroupCount {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int GroupCount {    System.int get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Number of center marks in a center mark set

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CenterMark::GroupCount.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Center Mark Set (C#)](Get_and_Set_Center_Marks_Set_Example_CSharp.htm)

[Get and Set Center Mark Set (VB.NET)](Get_and_Set_Center_Marks_Set_Example_VBNET.htm)

[Get and Set Center Mark Set (VBA)](Get_and_Set_Center_Marks_Set_Example_VBA.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the center mark is in a center mark set (i.e., a linear or circular pattern), then:

* you can only change the length of the arms of any of the center marks in that pattern; you cannot change any other properties of those center marks. Call [ICenterMark::IsGrouped](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~IsGrouped.html) to determine if a center mark is in a center mark set.* use this property to get a range of valid values for [ICenterMark::GetExtendedLength](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~GetExtendedLength.html)'s and [ICenterMark::SetExtendedLength](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~SetExtendedLength.html)'s GroupID parameter. You can use a value from 0 to the number of center marks in a center mark set for the GroupID parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html)

[ICenterMark Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0