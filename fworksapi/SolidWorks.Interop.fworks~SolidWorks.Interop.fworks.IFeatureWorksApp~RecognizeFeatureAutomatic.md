<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureAutomatic.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| RecognizeFeatureAutomatic Method (IFeatureWorksApp) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) > [IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html) : RecognizeFeatureAutomatic Method (IFeatureWorksApp) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*options*
:   Automatic options as defined by [fwAutomaticRecognitionOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwAutomaticRecognitionOptions_e.html)

Recognizes imported features automatically in a SOLIDWORKS part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RecognizeFeatureAutomatic( _    ByVal options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureWorksApp Dim options As System.Integer Dim value As System.Integer   value = instance.RecognizeFeatureAutomatic(options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RecognizeFeatureAutomatic(     System.int options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RecognizeFeatureAutomatic(  &   System.int options ) ``` | |

#### Parameters

*options*
:   Automatic options as defined by [fwAutomaticRecognitionOptions\_e](SOLIDWORKS.Interop.fworks~SOLIDWORKS.Interop.fworks.fwAutomaticRecognitionOptions_e.html)

#### Return Value

Number of features recognized

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureWorksApp::RecognizeFeatureAutomatic.

# ![](dotnetimages/collapse.gif)Example

[Recognizing Features Automatically (VBA)](Recognizing_Features_Automatically.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureWorksApp Interface](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp.html)

[IFeatureWorksApp Members](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp_members.html)

[IFeatureWorksApp::RecognizeFeatureInteractive Method](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.IFeatureWorksApp~RecognizeFeatureInteractive.html)

# ![](dotnetimages/collapse.gif)Availability

FeatureWorks API 2004 FCS