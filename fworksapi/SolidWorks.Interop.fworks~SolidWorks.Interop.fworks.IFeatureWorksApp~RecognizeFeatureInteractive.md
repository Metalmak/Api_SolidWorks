<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureInteractive.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| RecognizeFeatureInteractive Method (IFeatureWorksApp) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) > [IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html) : RecognizeFeatureInteractive Method (IFeatureWorksApp) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FeatureType*
:   Type of body or sheet metal feature to recognize

*options*
:   Interactive options as defined by [fwInteractiveRecognitionOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwInteractiveRecognitionOptions_e.html)

Recognizes imported features interactively in a SOLIDWORKS part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RecognizeFeatureInteractive( _    ByVal FeatureType As System.String, _    ByVal options As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureWorksApp Dim FeatureType As System.String Dim options As System.Integer Dim value As System.Boolean   value = instance.RecognizeFeatureInteractive(FeatureType, options) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RecognizeFeatureInteractive(     System.string FeatureType,    System.int options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RecognizeFeatureInteractive(  &   System.String^ FeatureType, &   System.int options ) ``` | |

#### Parameters

*FeatureType*
:   Type of body or sheet metal feature to recognize

*options*
:   Interactive options as defined by [fwInteractiveRecognitionOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwInteractiveRecognitionOptions_e.html)

#### Return Value

True if the feature is recognized, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureWorksApp::RecognizeFeatureInteractive.

# ![](dotnetimages/collapse.gif)Example

[Recognizing Features Interactively (VBA)](Recognizing_Features_Interactively.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html)

[IFeatureWorksApp Members](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp_members.html)

[IFeatureWorksApp::RecognizeFeatureAutomatic Method](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureAutomatic.html)

# ![](dotnetimages/collapse.gif)Availability

FeatureWorks API 2004 FCS