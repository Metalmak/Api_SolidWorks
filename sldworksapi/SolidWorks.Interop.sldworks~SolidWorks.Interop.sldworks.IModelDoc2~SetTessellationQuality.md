<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetTessellationQuality.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetTessellationQuality Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetTessellationQuality Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*QualityNum*
:   0 < Shaded-display image quality number < 106 (see **Remarks**)

Sets the shaded-display image quality number for the current document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetTessellationQuality( _    ByVal QualityNum As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim QualityNum As System.Integer   instance.SetTessellationQuality(QualityNum) ``` | |

| C# |  |
| --- | --- |
| ``` void SetTessellationQuality(     System.int QualityNum ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetTessellationQuality(  &   System.int QualityNum ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*QualityNum*
:   0 < Shaded-display image quality number < 106 (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetTessellationQuality.

# ![](dotnetimages/collapse.gif)Remarks

QualityNum is the degree of tessellation of curved surfaces for shaded rendering output. **Tools > Options > Document Properties > Image Quality** includes a field that sets the maximum chordal deviation. QualityNum and the maximum chordal deviation (in meters) are coupled and inversely proportional as follows:

*var* = *TessMin* + *QualityNum*\*((*TessMax*-*TessMin*)/100)

*Deviation* = 0.025 \* (*BodyDiameter* \* 2) / *var*;

where:

* *TessMin* = 6* *TessMax* = 166* 0 < *QualityNum* < 106* *BodyDiameter* is the diagonal distance across the bounds of the part box. See [IPartDoc::GetPartBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~GetPartBox.html) or [IPartDoc::IGetPartBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~IGetPartBox.html) for more information.

There are two ways to set the image quality for assemblies using the API. You can either:

* Call this method

    - or -

* Set swUserPreferenceIntegerValue\_e.swImageQualityShaded* Set swUserPreferenceDoubleValue\_e.swImageQualityShadedDeviation

Before doing either, you must set swUserPreferenceToggle\_e.swImageQualityApplyToAllReferencedPartDoc to true in order to affect the image quality of the assembly.

Call [IModelView::GraphicsRedraw](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~GraphicsRedraw.html) after calling this method to update the part.

**NOTE:** Setting the degree of tessellation to a higher value results in:

* finer tessellation,* increased file size,* slower graphics performance, and* increased memory usage.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetTessellationQuality Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetTessellationQuality.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0