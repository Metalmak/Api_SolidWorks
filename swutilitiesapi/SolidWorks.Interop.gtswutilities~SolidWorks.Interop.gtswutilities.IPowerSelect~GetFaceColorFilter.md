<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~GetFaceColorFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetFaceColorFilter Method (IPowerSelect) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : GetFaceColorFilter Method (IPowerSelect) |

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

Gets the Face color filter set in this PowerSelect session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFaceColorFilter( _    ByRef Red As System.Double, _    ByRef Green As System.Double, _    ByRef Blue As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim Red As System.Double Dim Green As System.Double Dim Blue As System.Double Dim value As System.Integer   value = instance.GetFaceColorFilter(Red, Green, Blue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetFaceColorFilter(     out System.double Red,    out System.double Green,    out System.double Blue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetFaceColorFilter(  &   [Out] System.double Red, &   [Out] System.double Green, &   [Out] System.double Blue ) ``` | |

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

See IPowerSelect::GetFaceColorFilter.

# ![](dotnetimages/collapse.gif)Example

[Select and Get Number of Edges, Loops, Faces, and Features (VBA)](Select_and_Get_Number_of_Edges%2C_Loops%2C_Faces%2C_and_Features_Example_VB6.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

[IPowerSelect::SetFaceColorFilter Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetFaceColorFilter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS