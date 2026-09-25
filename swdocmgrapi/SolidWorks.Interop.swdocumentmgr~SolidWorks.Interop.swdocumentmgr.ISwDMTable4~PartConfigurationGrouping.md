<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable4~PartConfigurationGrouping.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| PartConfigurationGrouping Property (ISwDMTable4) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMTable4 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable4.html) : PartConfigurationGrouping Property (ISwDMTable4) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the part configuration grouping for the bill of materials (BOM) table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property PartConfigurationGrouping As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMTable4 Dim value As System.Integer   value = instance.PartConfigurationGrouping ``` | |

| C# |  |
| --- | --- |
| ``` System.int PartConfigurationGrouping {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int PartConfigurationGrouping {    System.int get(); } ``` | |

#### Property Value

Part configuration grouping as defined in [swDMPartConfigurationGrouping](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.swDMPartConfigurationGrouping.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMTable4::PartConfigurationGrouping.

# ![](dotnetimages/collapse.gif)Example

[Get BOM Tables (C#)](Get_BOM_Tables_Example_CSharp.htm)

[Get BOM Tables (VB.NET)](Get_BOM_Tables_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Requirements

This property only supports model documents saved in SOLIDWORKS 2012 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMTable4 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable4.html)

[ISwDMTable4 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable4_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2012 SP0