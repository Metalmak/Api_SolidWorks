<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~CreateFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| CreateFeatures Method (IFeatureWorksApp) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) > [IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html) : CreateFeatures Method (IFeatureWorksApp) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CreationOptions*
:   Options as defined by [fwFeatureCreationOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwFeatureCreationOptions_e.html)

Creates recognized imported features in a SOLIDWORKS part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFeatures( _    ByVal CreationOptions As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureWorksApp Dim CreationOptions As System.Short Dim value As System.Boolean   value = instance.CreateFeatures(CreationOptions) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateFeatures(     System.short CreationOptions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateFeatures(  &   System.short CreationOptions ) ``` | |

#### Parameters

*CreationOptions*
:   Options as defined by [fwFeatureCreationOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwFeatureCreationOptions_e.html)

#### Return Value

True if the feature is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureWorksApp::CreateFeatures.

# ![](dotnetimages/collapse.gif)Example

[Recognizing Features Automatically (VBA)](Recognizing_Features_Automatically.htm)

[Recognizing Features Interactively (VBA)](Recognizing_Features_Interactively.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html)

[IFeatureWorksApp Members](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp_members.html)

[IFeatureWorksApp::RecognizeFeatureAutomatic Method](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureAutomatic.html)

[IFeatureWorksApp::RecognizeFeatureInteractive Method](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureInteractive.html)

# ![](dotnetimages/collapse.gif)Availability

FeaturesWorks API 2004 FCS