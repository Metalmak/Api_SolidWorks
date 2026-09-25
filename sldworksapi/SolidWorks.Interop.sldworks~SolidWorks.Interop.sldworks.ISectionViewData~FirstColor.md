<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~FirstColor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FirstColor Property (ISectionViewData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html) : FirstColor Property (ISectionViewData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the first color of the section view in the part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FirstColor As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISectionViewData Dim value As System.Integer   instance.FirstColor = value   value = instance.FirstColor ``` | |

| C# |  |
| --- | --- |
| ``` System.int FirstColor {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int FirstColor {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

RGB value of the first color

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SectionViewData::FirstColor.

# ![](dotnetimages/collapse.gif)Example

[Create Section View in Model (C#)](Create_Section_View_in_Model_Example_CSharp.htm)

[Create Section View in Model (VB.NET)](Create_Section_View_in_Model_Example_VBNET.htm)

[Create Section View in Model (VBA)](Create_Section_View_in_Model_Example_VB.htm)

[Get Section View Data (C#)](Get_Section_View_Data_Example_CSharp.htm)

[Get Section View Data (VB.NET)](Get_Section_View_Data_Example_VBNET.htm)

[Get Section View Data (VBA)](Get_Section_View_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [ISectionViewData::ShowSectionCap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISectionViewData~ShowSectionCap.html) to display the caps of section views and [ISectionView::KeepCapColor](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISectionViewData~KeepCapColor.html) to color them.

# ![](dotnetimages/collapse.gif)See Also

####

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)

[ISectionViewData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData_members.html)

[ISectionViewData::SecondColor Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~SecondColor.html)

[ISectionViewData::ThirdColor Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~ThirdColor.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0