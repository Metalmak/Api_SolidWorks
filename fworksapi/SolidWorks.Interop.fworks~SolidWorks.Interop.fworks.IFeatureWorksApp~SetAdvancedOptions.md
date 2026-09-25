<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~SetAdvancedOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| SetAdvancedOptions Method (IFeatureWorksApp) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) > [IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html) : SetAdvancedOptions Method (IFeatureWorksApp) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*options*
:   Advanced options as defined in [fwAdvancedOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwAdvancedOptions_e.html)

Set the specified advanced options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAdvancedOptions( _    ByVal options As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureWorksApp Dim options As System.Short Dim value As System.Boolean   value = instance.SetAdvancedOptions(options) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetAdvancedOptions(     System.short options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetAdvancedOptions(  &   System.short options ) ``` | |

#### Parameters

*options*
:   Advanced options as defined in [fwAdvancedOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwAdvancedOptions_e.html)

#### Return Value

True if the advanced options are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureWorksApp::SetAdvancedOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html)

[IFeatureWorksApp Members](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp_members.html)

# ![](dotnetimages/collapse.gif)Availability

FeatureWorks API 2009 FCS