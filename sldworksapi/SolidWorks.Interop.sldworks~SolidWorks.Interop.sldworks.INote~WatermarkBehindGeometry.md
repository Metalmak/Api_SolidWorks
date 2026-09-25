<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkBehindGeometry.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| WatermarkBehindGeometry Property (INote) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : WatermarkBehindGeometry Property (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to place this note, specified to be a watermark, behind the geometry in a part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property WatermarkBehindGeometry As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim value As System.Boolean   instance.WatermarkBehindGeometry = value   value = instance.WatermarkBehindGeometry ``` | |

| C# |  |
| --- | --- |
| ``` System.bool WatermarkBehindGeometry {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool WatermarkBehindGeometry {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to place this note behind the geometry in a part or assembly, false to place this note in front of the geometry in a part or assembly

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::WatermarkBehindGeometry.

# ![](dotnetimages/collapse.gif)Example

[Add Watermark to Part (C#)](Add_Watermark_to_Part_Example_CSharp.htm)

[Add Watermark to Part (VB.NET)](Add_Watermark_to_Part_Example_VBNET.htm)

[Add Watermark to Part (VBA)](Add_Watermark_to_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is only available when [INote::WatermarkNote](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkNote.html) is true.

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[INote::WatermarkTransparencyLevel Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~WatermarkTransparencyLevel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0