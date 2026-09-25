<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetShowHiddenEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SetShowHiddenEntities Method (IPowerSelect) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : SetShowHiddenEntities Method (IPowerSelect) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*varShow*
:   True to show both non-hidden and hidden entities, false to show only non-hidden entities

Sets whether to show both non-hidden and hidden entities or to show only non-hidden entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetShowHiddenEntities( _    ByVal varShow As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim varShow As System.Boolean Dim value As System.Integer   value = instance.SetShowHiddenEntities(varShow) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetShowHiddenEntities(     System.bool varShow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetShowHiddenEntities(  &   System.bool varShow ) ``` | |

#### Parameters

*varShow*
:   True to show both non-hidden and hidden entities, false to show only non-hidden entities

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IPowerSelect::SetShowHiddenEntities.

# ![](dotnetimages/collapse.gif)Remarks

Use [IPowerSelect::GetShowHiddenEntities](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect~GetShowHiddenEntities.html) to get whether or not to show both non-hidden and hidden entities or to show only non-hidden entities.

This method is the equivalent to the user-interface Show features of hidden body option on the Power Select dialog.

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2006 FCS