<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager~CaptureProbedResultPlotAsPNGImage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CaptureProbedResultPlotAsPNGImage Method (ICWResultsProbeManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html) : CaptureProbedResultPlotAsPNGImage Method (ICWResultsProbeManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SImageFolder*
:   Name of folder to which to save the image

*SImageName*
:   Name of file to which to save the image

Saves the probed results plot as a PNG image in the specified file and folder.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CaptureProbedResultPlotAsPNGImage( _    ByVal SImageFolder As System.String, _    ByVal SImageName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResultsProbeManager Dim SImageFolder As System.String Dim SImageName As System.String Dim value As System.Integer   value = instance.CaptureProbedResultPlotAsPNGImage(SImageFolder, SImageName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CaptureProbedResultPlotAsPNGImage(     System.string SImageFolder,    System.string SImageName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CaptureProbedResultPlotAsPNGImage(  &   System.String^ SImageFolder, &   System.String^ SImageName ) ``` | |

#### Parameters

*SImageFolder*
:   Name of folder to which to save the image

*SImageName*
:   Name of file to which to save the image

#### Return Value

Error code as defined in [swsProbePostResultErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResultsProbeManager::CaptureProbedResultPlotAsPNGImage.

# ![](dotnetimages/collapse.gif)Example

See the [ICWResultsProbeManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResultsProbeManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager.html)

[ICWResultsProbeManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0