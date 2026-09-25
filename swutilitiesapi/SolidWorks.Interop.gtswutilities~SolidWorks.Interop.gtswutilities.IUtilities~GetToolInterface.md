<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilities~GetToolInterface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetToolInterface Method (IUtilities) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IUtilities Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilities.html) : GetToolInterface Method (IUtilities) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*toolname*
:   Tool ID as defined by [gtSwTools\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtSwTools_e.html)

*lErrorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

Gets a pointer to the SOLIDWORKS Utilities tool.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetToolInterface( _    ByVal toolname As System.Integer, _    ByRef lErrorcode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUtilities Dim toolname As System.Integer Dim lErrorcode As System.Integer Dim value As System.Object   value = instance.GetToolInterface(toolname, lErrorcode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetToolInterface(     System.int toolname,    out System.int lErrorcode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetToolInterface(  &   System.int toolname, &   [Out] System.int lErrorcode ) ``` | |

#### Parameters

*toolname*
:   Tool ID as defined by [gtSwTools\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtSwTools_e.html)

*lErrorcode*
:   Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

#### Return Value

Pointer to the SOLIDWORKS Utilities tool interface

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IUtilities::GetToolInterface.

# ![](dotnetimages/collapse.gif)Example

[Analyze Geometry (VBA)](Analyze_Geometry_VB6.htm)

[Compare Documents (VBA)](Compare_Documents_VB6.htm)

[Compare Features (VBA)](Compare_Features_VB6.htm)

[Compare Geometry (VBA)](Compare_Geometry_VB6.htm)

[Paint Features (VBA)](Paint_Features_VB6.htm)

[Compare Geometry (VB.NET)](Compare_Geometry_VBNET.htm)

[Compare Geometry (C#)](Compare_Geometry_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IUtilities Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilities.html)

[IUtilities Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilities_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS