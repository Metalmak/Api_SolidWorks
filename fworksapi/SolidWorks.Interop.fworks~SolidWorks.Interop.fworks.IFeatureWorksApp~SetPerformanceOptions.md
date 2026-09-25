<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~SetPerformanceOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| SetPerformanceOptions Method (IFeatureWorksApp) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) > [IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html) : SetPerformanceOptions Method (IFeatureWorksApp) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*options*
:   Performance options as defined by [fwPerformanceOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwPerformanceOptions_e.html)

Sets the desired performance options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPerformanceOptions( _    ByVal options As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureWorksApp Dim options As System.Short Dim value As System.Boolean   value = instance.SetPerformanceOptions(options) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPerformanceOptions(     System.short options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPerformanceOptions(  &   System.short options ) ``` | |

#### Parameters

*options*
:   Performance options as defined by [fwPerformanceOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwPerformanceOptions_e.html)

#### Return Value

True if the performance options are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureWorksApp::SetPerformanceOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html)

[IFeatureWorksApp Members](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp_members.html)

# ![](dotnetimages/collapse.gif)Availability

FeatureWorks API 2004 FCS