<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager~ShowAnnotationsOnNodesOrElems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ShowAnnotationsOnNodesOrElems Method (ICWResultsProbeManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html) : ShowAnnotationsOnNodesOrElems Method (ICWResultsProbeManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SSelectedNodesOrElems*
:   Comma-delimited string of nodes or elements, e.g., "1,25,30-35"

*ArrayAnnotationWarnings*
:   Array of warnings for specified nodes or elements as defined in [swsProbePostResultNodeElementSelectionWarning\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultNodeElementSelectionWarning_e.html)

Shows results probe annotations for the specified nodes or elements.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowAnnotationsOnNodesOrElems( _    ByVal SSelectedNodesOrElems As System.String, _    ByRef ArrayAnnotationWarnings As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResultsProbeManager Dim SSelectedNodesOrElems As System.String Dim ArrayAnnotationWarnings As System.Object Dim value As System.Integer   value = instance.ShowAnnotationsOnNodesOrElems(SSelectedNodesOrElems, ArrayAnnotationWarnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowAnnotationsOnNodesOrElems(     System.string SSelectedNodesOrElems,    out System.object ArrayAnnotationWarnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ShowAnnotationsOnNodesOrElems(  &   System.String^ SSelectedNodesOrElems, &   [Out] System.Object^ ArrayAnnotationWarnings ) ``` | |

#### Parameters

*SSelectedNodesOrElems*
:   Comma-delimited string of nodes or elements, e.g., "1,25,30-35"

*ArrayAnnotationWarnings*
:   Array of warnings for specified nodes or elements as defined in [swsProbePostResultNodeElementSelectionWarning\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultNodeElementSelectionWarning_e.html)

#### Return Value

0 if successful; otherwise error code as defined in [swsProbePostResultErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResultsProbeManager::ShowAnnotationsOnNodesOrElems.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html)

[ICWResultsProbeManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP3