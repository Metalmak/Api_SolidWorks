<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetIndependentViewPort.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetIndependentViewPort Method (IMBD3DPdfData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMBD3DPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html) : SetIndependentViewPort Method (IMBD3DPdfData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ViewName*
:   Name of the view (e.g., "Top View" or "\*Top")

Sets the specified view for an independent viewport for the SOLIDWORKS MBD 3D PDF.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetIndependentViewPort( _    ByVal ViewName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMBD3DPdfData Dim ViewName As System.String Dim value As System.Boolean   value = instance.SetIndependentViewPort(ViewName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetIndependentViewPort(     System.string ViewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetIndependentViewPort(  &   System.String^ ViewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ViewName*
:   Name of the view (e.g., "Top View" or "\*Top")

#### Return Value

True if the specified view is set for an independent viewport for the SOLIDWORKS MBD 3D PDF, false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MBD3DPdfData::SetIndependentViewPort.

# ![](dotnetimages/collapse.gif)Example

[Set Independent Viewport for MBD 3D PDF (C#)](Set_Independent_Viewport_for_MBD_3D_PDF_Example_CSharp.htm)

[Set Independent Viewport for MBD 3D PDF (VB.NET)](Set_Independent_Viewport_for_MBD_3D_PDF_Example_VBNET.htm)

[Set Independent Viewport for MBD 3D PDF (VBA)](Set_Independent_Viewport_for_MBD_3D_PDF_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The [theme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) for the SOLIDWORKS MBD 3D PDF must contain an independent viewport. See the examples for instructions on how to add an independent viewport to a theme and how to set a view for that independent viewport.

# ![](dotnetimages/collapse.gif)See Also

####

[IMBD3DPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html)

[IMBD3DPdfData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0