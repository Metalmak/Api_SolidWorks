<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15~ShowChildComponentsInBOM2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| ShowChildComponentsInBOM2 Property (ISwDMConfiguration15) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration15 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15.html) : ShowChildComponentsInBOM2 Property (ISwDMConfiguration15) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether to show child components in the bill of materials (BOM) for this configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ShowChildComponentsInBOM2 As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration15 Dim value As System.Integer   instance.ShowChildComponentsInBOM2 = value   value = instance.ShowChildComponentsInBOM2 ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowChildComponentsInBOM2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ShowChildComponentsInBOM2 {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Show child components in BOM as defined in [swDmShowChildComponentsInBOMResult](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.swDmShowChildComponentsInBOMResult.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration15::ShowChildComponentsInBOM2.

# ![](dotnetimages/collapse.gif)Remarks

This property only supports documents saved in SOLIDWORKS 2009 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration15 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15.html)

[ISwDMConfiguration15 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2018 SP0