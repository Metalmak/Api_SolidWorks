<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxResultsEquationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxResultsEquationValues Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxResultsEquationValues Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SResultsEquation*
:   Results equation

*BValueByElem*
:   True to plot element values, false to plot node values

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*NStepNumber*
:   Number of solution step to plot

*NShellOptions*
:   Shell face as defined in [swsShellFace\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsShellFace_e.html); valid only for shell and mixed mesh models

*ErrorCode*
:   Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

Gets the algebraic minimum and maximum from the plot of the specified results equation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxResultsEquationValues( _    ByVal SResultsEquation As System.String, _    ByVal BValueByElem As System.Boolean, _    ByVal NUnits As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal NShellOptions As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SResultsEquation As System.String Dim BValueByElem As System.Boolean Dim NUnits As System.Integer Dim NStepNumber As System.Integer Dim NShellOptions As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxResultsEquationValues(SResultsEquation, BValueByElem, NUnits, NStepNumber, NShellOptions, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxResultsEquationValues(     System.string SResultsEquation,    System.bool BValueByElem,    System.int NUnits,    System.int NStepNumber,    System.int NShellOptions,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxResultsEquationValues(  &   System.String^ SResultsEquation, &   System.bool BValueByElem, &   System.int NUnits, &   System.int NStepNumber, &   System.int NShellOptions, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SResultsEquation*
:   Results equation

*BValueByElem*
:   True to plot element values, false to plot node values

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*NStepNumber*
:   Number of solution step to plot

*NShellOptions*
:   Shell face as defined in [swsShellFace\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsShellFace_e.html); valid only for shell and mixed mesh models

*ErrorCode*
:   Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

#### Return Value

Array (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxResultsEquationValues.

# ![](dotnetimages/collapse.gif)Example

[Create Results Equation Plot (VBA)](Create_Results_Equation_Plot_Example_VB.htm)

[Create Results Equation Plot (VB.NET)](Create_Results_Equation_Plot_Example_VBNET.htm)

[Create Results Equation Plot (C#)](Create_Results_Equation_Plot_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns the following array:

{

*node\_or\_element\_with\_minimum\_value*,

*minimum\_value*,

*node\_or\_element\_with\_maximum\_value*,

*maximum\_value*

},

where the nodes/elements are integer indexes, and the values are in scientific notation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::CreateResultsEquationPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateResultsEquationPlot.html)

[ICWResults::GetResultsEquationValuesForEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetResultsEquationValuesForEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0