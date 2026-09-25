<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultFrequencyOrBucklingStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddDefaultFrequencyOrBucklingStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : AddDefaultFrequencyOrBucklingStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BAllModeShapes*
:   True to create plots for all mode shapes, false to create plots for the first NDefMaxModeShapeValue mode shapes

*NDefMaxModeShapeValue*
:   Maximum number of mode shapes to plot; valid only if BAllModeShapes is false

*BDisplacement*
:   True to plot displacement, false to not

*NDisplacementValue*
:   Type of displacement result to plot as defined by [swsFrequencyBucklingResultDisplacementComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFrequencyBucklingResultDisplacementComponentTypes_e.html)

Specifies a default frequency or buckling study result plot for the active document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDefaultFrequencyOrBucklingStudyPlot( _    ByVal BAllModeShapes As System.Boolean, _    ByVal NDefMaxModeShapeValue As System.Integer, _    ByVal BDisplacement As System.Boolean, _    ByVal NDisplacementValue As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim BAllModeShapes As System.Boolean Dim NDefMaxModeShapeValue As System.Integer Dim BDisplacement As System.Boolean Dim NDisplacementValue As System.Integer Dim value As System.Integer   value = instance.AddDefaultFrequencyOrBucklingStudyPlot(BAllModeShapes, NDefMaxModeShapeValue, BDisplacement, NDisplacementValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddDefaultFrequencyOrBucklingStudyPlot(     System.bool BAllModeShapes,    System.int NDefMaxModeShapeValue,    System.bool BDisplacement,    System.int NDisplacementValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddDefaultFrequencyOrBucklingStudyPlot(  &   System.bool BAllModeShapes, &   System.int NDefMaxModeShapeValue, &   System.bool BDisplacement, &   System.int NDisplacementValue ) ``` | |

#### Parameters

*BAllModeShapes*
:   True to create plots for all mode shapes, false to create plots for the first NDefMaxModeShapeValue mode shapes

*NDefMaxModeShapeValue*
:   Maximum number of mode shapes to plot; valid only if BAllModeShapes is false

*BDisplacement*
:   True to plot displacement, false to not

*NDisplacementValue*
:   Type of displacement result to plot as defined by [swsFrequencyBucklingResultDisplacementComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFrequencyBucklingResultDisplacementComponentTypes_e.html)

#### Return Value

Error code as defined by [swsAddDefaultFrequencyOrBucklingStudyPlotResultError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAddDefaultFrequencyOrBucklingStudyPlotResultError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::AddDefaultFrequencyOrBucklingStudyPlot.

# ![](dotnetimages/collapse.gif)Example

[Create Frequency Study with Solid Mesh (VBA)](Create_Frequency_Study_with_Solid_Mesh_Example_VB.htm)

[Create Frequency Study with Solid Mesh (VB.NET)](Create_Frequency_Study_with_Solid_Mesh_Example_VBNET.htm)

[Create Frequency Study with Solid Mesh (C#)](Create_Frequency_Study_with_Solid_Mesh_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0