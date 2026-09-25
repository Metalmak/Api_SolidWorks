<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~GetFeatureColorFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetFeatureColorFilter Method (IPowerSelect) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : GetFeatureColorFilter Method (IPowerSelect) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Red*
:   <=0.0  to <= 1.0

*Green*
:   <=0.0  to <= 1.0

*Blue*
:   <=0.0  to <= 1.0

Gets the Feature color filter set in this PowerSelect session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFeatureColorFilter( _    ByRef Red As System.Double, _    ByRef Green As System.Double, _    ByRef Blue As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim Red As System.Double Dim Green As System.Double Dim Blue As System.Double Dim value As System.Integer   value = instance.GetFeatureColorFilter(Red, Green, Blue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetFeatureColorFilter(     out System.double Red,    out System.double Green,    out System.double Blue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetFeatureColorFilter(  &   [Out] System.double Red, &   [Out] System.double Green, &   [Out] System.double Blue ) ``` | |

#### Parameters

*Red*
:   <=0.0  to <= 1.0

*Green*
:   <=0.0  to <= 1.0

*Blue*
:   <=0.0  to <= 1.0

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IPowerSelect::GetFeatureColorFilter.

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

[IPowerSelect::SetFeatureColorFilter Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetFeatureColorFilter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS