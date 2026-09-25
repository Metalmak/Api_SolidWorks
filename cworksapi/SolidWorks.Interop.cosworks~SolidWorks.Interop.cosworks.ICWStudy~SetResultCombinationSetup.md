<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~SetResultCombinationSetup.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetResultCombinationSetup Method (ICWStudy) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : SetResultCombinationSetup Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NOption*
:   Type of result combination as defined in [swsPVResultCombinationType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPVResultCombinationType_e.html)

*NItems*
:   Number of elements in the MultiplicationFactors and StudyNames arrays

*MultiplicationFactors*
:   Array of multiplication factors; valid only if NOption = swsPVResultCombinationType\_e.swsPVResultCombinationType\_Linear

*StudyNames*
:   Array of names of the static studies whose results you want to combine; if NOption = swsPVResultCombinationType\_e.swsPVResultCombinationType\_Linear, the elements of MultiplicationFactors are coefficients of the linear combination of the static study results

Sets the result combination setup for this Pressure Vessel Design study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetResultCombinationSetup( _    ByVal NOption As System.Integer, _    ByVal NItems As System.Integer, _    ByVal MultiplicationFactors As System.Object, _    ByVal StudyNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim NOption As System.Integer Dim NItems As System.Integer Dim MultiplicationFactors As System.Object Dim StudyNames As System.Object Dim value As System.Integer   value = instance.SetResultCombinationSetup(NOption, NItems, MultiplicationFactors, StudyNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetResultCombinationSetup(     System.int NOption,    System.int NItems,    System.object MultiplicationFactors,    System.object StudyNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetResultCombinationSetup(  &   System.int NOption, &   System.int NItems, &   System.Object^ MultiplicationFactors, &   System.Object^ StudyNames ) ``` | |

#### Parameters

*NOption*
:   Type of result combination as defined in [swsPVResultCombinationType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPVResultCombinationType_e.html)

*NItems*
:   Number of elements in the MultiplicationFactors and StudyNames arrays

*MultiplicationFactors*
:   Array of multiplication factors; valid only if NOption = swsPVResultCombinationType\_e.swsPVResultCombinationType\_Linear

*StudyNames*
:   Array of names of the static studies whose results you want to combine; if NOption = swsPVResultCombinationType\_e.swsPVResultCombinationType\_Linear, the elements of MultiplicationFactors are coefficients of the linear combination of the static study results

#### Return Value

Error as defined in [swsPVResultCombinationError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPVResultCombinationError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::SetResultCombinationSetup.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0