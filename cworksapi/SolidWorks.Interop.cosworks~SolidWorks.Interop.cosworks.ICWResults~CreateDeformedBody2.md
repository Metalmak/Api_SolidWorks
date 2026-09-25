<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateDeformedBody2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateDeformedBody2 Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : CreateDeformedBody2 Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCreateAs*
:   Save option as defined in [swsCreateDeformedBodyOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyOption_e.html)

*NAdvOption*
:   Advanced save option as defined in [swsCreateDeformedBodyAdvancedOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyAdvancedOption_e.html)

*NStepNumber*
:   1 for a static study or a valid step number for a nonlinear study (see **Remarks**)

*SName*
:   Name of the deformed shape to save

*SFolderName*
:   Path name of folder in which to save SName

Saves the deformed shape that results from running a [static](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) or [nonlinear](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWNonLinearStudyOptions.html) study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateDeformedBody2( _    ByVal NCreateAs As System.Integer, _    ByVal NAdvOption As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal SName As System.String, _    ByVal SFolderName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NCreateAs As System.Integer Dim NAdvOption As System.Integer Dim NStepNumber As System.Integer Dim SName As System.String Dim SFolderName As System.String Dim value As System.Integer   value = instance.CreateDeformedBody2(NCreateAs, NAdvOption, NStepNumber, SName, SFolderName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateDeformedBody2(     System.int NCreateAs,    System.int NAdvOption,    System.int NStepNumber,    System.string SName,    System.string SFolderName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateDeformedBody2(  &   System.int NCreateAs, &   System.int NAdvOption, &   System.int NStepNumber, &   System.String^ SName, &   System.String^ SFolderName ) ``` | |

#### Parameters

*NCreateAs*
:   Save option as defined in [swsCreateDeformedBodyOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyOption_e.html)

*NAdvOption*
:   Advanced save option as defined in [swsCreateDeformedBodyAdvancedOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyAdvancedOption_e.html)

*NStepNumber*
:   1 for a static study or a valid step number for a nonlinear study (see **Remarks**)

*SName*
:   Name of the deformed shape to save

*SFolderName*
:   Path name of folder in which to save SName

#### Return Value

0 if successful, otherwise error code as defined in [swsCreateDeformedBodyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::CreateDeformedBody2.

# ![](dotnetimages/collapse.gif)Example

[Create Body From Deformed Shape (VBA)](Create_Body_From_Deformed_Shape_Example_VB.htm)

[Create Body From Deformed Shape (VB.NET)](Create_Body_From_Deformed_Shape_Example_VBNET.htm)

[Create Body From Deformed Shape (C#)](Create_Body_From_Deformed_Shape_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Deformed shapes of assembly documents are saved as multibody parts.

To populate NStepNumber for a nonlinear study, call [ICWResults::GetMaximumAvailableSteps](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMaximumAvailableSteps.html) to get the maximum number of steps in the nonlinear study.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetDeformedBodyFailedSewOption Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDeformedBodyFailedSewOption.html)

[ICWResults::SetDeformedBodyFailedSewOption Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetDeformedBodyFailedSewOption.html)

[ICWResults::GetDeformedCoord Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDeformedCoord.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0