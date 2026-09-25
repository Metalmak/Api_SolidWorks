<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PresetNewDrawingParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PresetNewDrawingParameters Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : PresetNewDrawingParameters Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DrawingTemplate*
:   Path and filename (.slddrt) of the drawing template to use

*ShowTemplate*
:   True to show the sheet format, false to not

    **NOTE:** Valid only for standard sheet sizes and when Width and Height are set to 0.

*Width*
:   Width of the drawing sheet

*Height*
:   Height of the drawing sheet

Presets the drawing template and sheet size parameters to avoid showing the Sheet Format/Size dialog when creating a new drawing document in the user-interface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PresetNewDrawingParameters( _    ByVal DrawingTemplate As System.String, _    ByVal ShowTemplate As System.Boolean, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DrawingTemplate As System.String Dim ShowTemplate As System.Boolean Dim Width As System.Double Dim Height As System.Double Dim value As System.Boolean   value = instance.PresetNewDrawingParameters(DrawingTemplate, ShowTemplate, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool PresetNewDrawingParameters(     System.string DrawingTemplate,    System.bool ShowTemplate,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool PresetNewDrawingParameters(  &   System.String^ DrawingTemplate, &   System.bool ShowTemplate, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DrawingTemplate*
:   Path and filename (.slddrt) of the drawing template to use

*ShowTemplate*
:   True to show the sheet format, false to not

    **NOTE:** Valid only for standard sheet sizes and when Width and Height are set to 0.

*Width*
:   Width of the drawing sheet

*Height*
:   Height of the drawing sheet

#### Return Value

True if the specified drawing template and sheet size parameters are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::PresetNewDrawingParameters.

# ![](dotnetimages/collapse.gif)Example

[Preset and Reset Template and Sheet Parameters for New Drawing Documents (VBA)](Preset_and_Reset_Template_and_Sheet_Parameters_for_New_Drawing_Documents_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To show the Sheet Format/Size dialog the next time a new drawing document is opened (SOLIDWORKS default behavior), call [ISldWorks::ResetPresetDrawingParameters](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ResetPresetDrawingParameters.html) after calling this method and opening a new drawing document.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0