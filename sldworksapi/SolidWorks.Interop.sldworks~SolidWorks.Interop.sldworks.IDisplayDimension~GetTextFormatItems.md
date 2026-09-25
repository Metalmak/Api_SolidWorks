<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetTextFormatItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTextFormatItems Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : GetTextFormatItems Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WhichText*
:   Portion of the display dimension text as defined in swDimensionTextParts\_e

*TokensDefinition*
:   Array of strings containing format symbols for the text portion specified in WhichText

*TokensEvaluated*
:   Array of strings containing evaluations of symbols in TokensDefinition

Gets the format tokens of the specified text portion of a multi-value display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTextFormatItems( _    ByVal WhichText As System.Integer, _    ByRef TokensDefinition As System.Object, _    ByRef TokensEvaluated As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim WhichText As System.Integer Dim TokensDefinition As System.Object Dim TokensEvaluated As System.Object Dim value As System.Integer   value = instance.GetTextFormatItems(WhichText, TokensDefinition, TokensEvaluated) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetTextFormatItems(     System.int WhichText,    out System.object TokensDefinition,    out System.object TokensEvaluated ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetTextFormatItems(  &   System.int WhichText, &   [Out] System.Object^ TokensDefinition, &   [Out] System.Object^ TokensEvaluated ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WhichText*
:   Portion of the display dimension text as defined in swDimensionTextParts\_e

*TokensDefinition*
:   Array of strings containing format symbols for the text portion specified in WhichText

*TokensEvaluated*
:   Array of strings containing evaluations of symbols in TokensDefinition

#### Return Value

Size of returned arrays

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::GetTextFormatItems.

# ![](dotnetimages/collapse.gif)Example

[Get Chamfer Display Dimension (C#)](Get_Chamfer_Display_Dimension_Example_CSharp.htm)

[Get Chamfer Display Dimension (VB.NET)](Get_Chamfer_Display_Dimension_Example_VBNET.htm)

[Get Chamfer Display Dimension (VBA)](Get_Chamfer_Display_Dimension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Each display dimension's PropertyManager page contains a section called Dimension Text that specifies the format of the displayed dimension. The format consists of function symbols or tokens enclosed within angle brackets (e.g., <DIM>), each of which connotes the function or definition of the value symbols that follow it.

This method retrieves all of the symbols, both function and value, for the portion of the display dimension text specified by WhichText. It also retrieves values for any symbols that can be evaluated in TokensDefinition.

**NOTE:** This method does not support [hole callouts](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~IsHoleCallout.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::GetText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0