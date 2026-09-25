<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkNote.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| WatermarkNote Property (INote) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : WatermarkNote Property (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether the note is a watermark in a part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property WatermarkNote As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim value As System.Boolean   instance.WatermarkNote = value   value = instance.WatermarkNote ``` | |

| C# |  |
| --- | --- |
| ``` System.bool WatermarkNote {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool WatermarkNote {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if the note is a watermark in a part or assembly, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::WatermarkNote.

# ![](dotnetimages/collapse.gif)Example

[Add Watermark to Part (C#)](Add_Watermark_to_Part_Example_CSharp.htm)

[Add Watermark to Part (VB.NET)](Add_Watermark_to_Part_Example_VBNET.htm)

[Add Watermark to Part (VBA)](Add_Watermark_to_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To add a watermark to a part or assembly document:

1. Open a part or assembly document.- Expand the **Annotations** folder in the FeatureManager design tree.- Right click **Notes Area** and click **Activate**.- Click **Insert > Annotations > Note**- Place the note in the graphics area, type the note text, and click **OK** in the Notes PropertyManager page.- Right-click the note and click **Watermark**.

Use [ISheet::BehindSheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~BehindSheet.html) to place a note on the sheet format behind a drawing sheet, which allows you to display the note as watermark in a drawing.

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[INote::WatermarkBehindGeometry Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkBehindGeometry.html)

[INote::WatermarkTransparencyLevel Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkTransparencyLevel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0