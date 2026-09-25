<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~ShowANSIInchLetterNumberDrillSizes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowANSIInchLetterNumberDrillSizes Property (IHoleTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html) : ShowANSIInchLetterNumberDrillSizes Property (IHoleTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to display hole sizes in this hole table using ANSI inch letters and drill numbers.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ShowANSIInchLetterNumberDrillSizes As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleTable Dim value As System.Boolean   instance.ShowANSIInchLetterNumberDrillSizes = value   value = instance.ShowANSIInchLetterNumberDrillSizes ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowANSIInchLetterNumberDrillSizes {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ShowANSIInchLetterNumberDrillSizes {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to display hole sizes using ANSI inch letters and drill numbers, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleTable::ShowANSIInchLetterNumberDrillSizes.

# ![](dotnetimages/collapse.gif)Example

[Get Labels of Datum Origin (VBA)](Get_Labels_of_Datum_Origin_Example_VB.htm)

[Get Labels of Datum Origin (VB.NET)](Get_Labels_of_Datum_Origin_Example_VBNET.htm)

[Get Labels of Datum Origin (C#)](Get_Labels_of_Datum_Origin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property:

* corresponds to the **Show ANSI inch letter and number drill sizes** option in the Scheme section of the Hole Table PropertyManager page in SOLIDWORKS.* is valid only for holes created with the Hole Wizard tool.* specifies whether to display hole sizes as ANSI inch letters or drill numbers, for example, A or #40.

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html)

[IHoleTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable_members.html)

[IHoleTable::CombineSameSize Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~CombineSameSize.html)

[IHoleTable::CombineTags Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~CombineTags.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0