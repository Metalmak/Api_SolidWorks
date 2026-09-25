<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetTimeOrFrequencyAtEachStep2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetTimeOrFrequencyAtEachStep2 Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetTimeOrFrequencyAtEachStep2 Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ForStressAndStrain*
:   -1 or true for stress or strain results, 0 or false for other results

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the times or frequencies for all solution steps or mode shapes in these results.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTimeOrFrequencyAtEachStep2( _    ByVal ForStressAndStrain As System.Boolean, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim ForStressAndStrain As System.Boolean Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetTimeOrFrequencyAtEachStep2(ForStressAndStrain, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetTimeOrFrequencyAtEachStep2(     System.bool ForStressAndStrain,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetTimeOrFrequencyAtEachStep2(  &   System.bool ForStressAndStrain, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ForStressAndStrain*
:   -1 or true for stress or strain results, 0 or false for other results

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

0-based array of:

* Times for time-domain studies

- or -

* Frequencies for frequency-domain studies

for all solution steps or mode shapes

# ![](dotnetimages/collapse.gif)Example

[Get Frequencies in Mode Shape Plots (VBA)](Get_Frequencies_in_Mode_Shape_Plots_Example_VB.htm)

[Get Frequencies in Mode Shape Plots (VB.NET)](Get_Frequencies_in_Mode_Shape_Plots_Example_VBNET.htm)

[Get Frequencies in Mode Shape Plots (C#)](Get_Free_Body_Forces_and_Moments_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30