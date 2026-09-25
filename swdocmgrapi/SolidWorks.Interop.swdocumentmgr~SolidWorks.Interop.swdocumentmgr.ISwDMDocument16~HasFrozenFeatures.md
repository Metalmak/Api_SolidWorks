<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument16~HasFrozenFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| HasFrozenFeatures Method (ISwDMDocument16) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument16 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument16.html) : HasFrozenFeatures Method (ISwDMDocument16) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FrozenFeatureNeedsUpdate*
:   True if the document has frozen features that need to be updated, false if not (see **Remarks**)

Gets whether the document has frozen features and whether those features need to be updated.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function HasFrozenFeatures( _    ByRef FrozenFeatureNeedsUpdate As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument16 Dim FrozenFeatureNeedsUpdate As System.Boolean Dim value As System.Boolean   value = instance.HasFrozenFeatures(FrozenFeatureNeedsUpdate) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HasFrozenFeatures(     out System.bool FrozenFeatureNeedsUpdate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool HasFrozenFeatures(  &   [Out] System.bool FrozenFeatureNeedsUpdate ) ``` | |

#### Parameters

*FrozenFeatureNeedsUpdate*
:   True if the document has frozen features that need to be updated, false if not (see **Remarks**)

#### Return Value

True if the document has frozen features, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument16::HasFrozenFeatures.

# ![](dotnetimages/collapse.gif)Example

[Get Whether Part Has Frozen Features (C#)](Get_Whether_Part_Has_Frozen_Features_Example_CSharp.htm)

[Get Whether Part Has Frozen Features (VB.NET)](Get_Whether_Part_Has_Frozen_Features_Example_vbnet.htm)

# ![](dotnetimages/collapse.gif)Remarks

The FrozenFeatureNeedsUpdate return value is only valid if the document has frozen features.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument16 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument16.html)

[ISwDMDocument16 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument16_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2012 SP0