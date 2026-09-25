<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11~ShowChildComponentsInBOM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| ShowChildComponentsInBOM Property (ISwDMConfiguration11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration11 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11.html) : ShowChildComponentsInBOM Property (ISwDMConfiguration11) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ISwDMConfiguration15::ShowChildComponentsInBOM2](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15~ShowChildComponentsInBOM2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ShowChildComponentsInBOM As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration11 Dim value As System.Integer   instance.ShowChildComponentsInBOM = value   value = instance.ShowChildComponentsInBOM ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowChildComponentsInBOM {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ShowChildComponentsInBOM {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Show child components in BOM as defined in [swDmShowChildComponetsInBOMResult](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.swDmShowChildComponentsInBOMResult.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration11::ShowChildComponentsInBOM.

# ![](dotnetimages/collapse.gif)Remarks

This property only supports documents saved in SOLIDWORKS 2009 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration11 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11.html)

[ISwDMConfiguration11 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11_members.html)