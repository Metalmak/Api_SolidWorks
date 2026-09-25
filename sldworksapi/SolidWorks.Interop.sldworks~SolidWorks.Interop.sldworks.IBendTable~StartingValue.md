<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable~StartingValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| StartingValue Property (IBendTable) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBendTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable.html) : StartingValue Property (IBendTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the starting datum tag for this bend table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property StartingValue As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBendTable Dim value As System.String   instance.StartingValue = value   value = instance.StartingValue ``` | |

| C# |  |
| --- | --- |
| ``` System.string StartingValue {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ StartingValue {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Starting datum tag (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BendTable::StartingValue.

# ![](dotnetimages/collapse.gif)Example

[Insert Bend Table (C#)](Insert_Bend_Table_Example_CSharp.htm)

[Insert Bend Table (VB.NET)](Insert_Bend_Table_Example_VBNET.htm)

[Insert Bend Table (VBA)](Insert_Bend_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property returns:

* Letter from A to Z, if [IBendTable::TagStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBendTable~TagStyle.html) is set to swBendTableTagStyle\_e.swBendTable\_AlphaNumericTags.* Positive integer, if [IBendTable::TagStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBendTable~TagStyle.html) is set to swBendTableTagStyle\_e.swBendTable\_NumericTags.

# ![](dotnetimages/collapse.gif)See Also

####

[IBendTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable.html)

[IBendTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0