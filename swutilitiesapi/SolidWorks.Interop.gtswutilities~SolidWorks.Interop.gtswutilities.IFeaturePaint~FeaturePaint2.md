<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFeaturePaint~FeaturePaint2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| FeaturePaint2 Method (IFeaturePaint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IFeaturePaint Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFeaturePaint.html) : FeaturePaint2 Method (IFeaturePaint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*sourcefeature*
:   <source feature name>@<path\filename>.sldprt

*targetfeature*
:   <target feature name>@<path\filename>.sldprt

*pasteappearance*
:   True if the source feature's parameters are copied to the target feature, false if not

Copies the source feature's parameters to the target feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeaturePaint2( _    ByVal sourcefeature As System.String, _    ByVal targetfeature As System.String, _    ByVal pasteappearance As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeaturePaint Dim sourcefeature As System.String Dim targetfeature As System.String Dim pasteappearance As System.Boolean Dim value As System.Integer   value = instance.FeaturePaint2(sourcefeature, targetfeature, pasteappearance) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeaturePaint2(     System.string sourcefeature,    System.string targetfeature,    System.bool pasteappearance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FeaturePaint2(  &   System.String^ sourcefeature, &   System.String^ targetfeature, &   System.bool pasteappearance ) ``` | |

#### Parameters

*sourcefeature*
:   <source feature name>@<path\filename>.sldprt

*targetfeature*
:   <target feature name>@<path\filename>.sldprt

*pasteappearance*
:   True if the source feature's parameters are copied to the target feature, false if not

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IFeaturePaint::FeaturePaint2.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeaturePaint Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFeaturePaint.html)

[IFeaturePaint Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFeaturePaint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS