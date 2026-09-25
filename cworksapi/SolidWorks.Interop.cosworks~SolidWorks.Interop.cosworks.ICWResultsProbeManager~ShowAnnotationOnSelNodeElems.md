<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager~ShowAnnotationOnSelNodeElems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ShowAnnotationOnSelNodeElems Method (ICWResultsProbeManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html) : ShowAnnotationOnSelNodeElems Method (ICWResultsProbeManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArraySelectedNodeElems*
:   Array of nodes or elements

*ArrayAnnotationWarnings*
:   Array of warnings for specified nodes or elements as defined in [swsProbePostResultNodeElementSelectionWarning\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultNodeElementSelectionWarning_e.html)

Obsoleted. Superseded by [ICWResultsProbeManager::ShowAnnotationsOnNodesOrElems](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager~ShowAnnotationsOnNodesOrElems.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowAnnotationOnSelNodeElems( _    ByVal ArraySelectedNodeElems As System.Object, _    ByRef ArrayAnnotationWarnings As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResultsProbeManager Dim ArraySelectedNodeElems As System.Object Dim ArrayAnnotationWarnings As System.Object Dim value As System.Integer   value = instance.ShowAnnotationOnSelNodeElems(ArraySelectedNodeElems, ArrayAnnotationWarnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ShowAnnotationOnSelNodeElems(     System.object ArraySelectedNodeElems,    out System.object ArrayAnnotationWarnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ShowAnnotationOnSelNodeElems(  &   System.Object^ ArraySelectedNodeElems, &   [Out] System.Object^ ArrayAnnotationWarnings ) ``` | |

#### Parameters

*ArraySelectedNodeElems*
:   Array of nodes or elements

*ArrayAnnotationWarnings*
:   Array of warnings for specified nodes or elements as defined in [swsProbePostResultNodeElementSelectionWarning\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultNodeElementSelectionWarning_e.html)

#### Return Value

Error code as defined in [swsProbePostResultErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResultsProbeManager::ShowAnnotationOnSelNodeElems.

# ![](dotnetimages/collapse.gif)Example

See the [ICWResultsProbeManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html)

[ICWResultsProbeManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0