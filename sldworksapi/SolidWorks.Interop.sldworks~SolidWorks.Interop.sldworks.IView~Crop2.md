<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~Crop2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Crop2 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : Crop2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*JaggedOutline*
:   True to use a jagged outline, false to not; only valid if NoOutline is false

*NoOutline*
:   True to not show an outline, false to show an outline

*ShapeIntensity*
:   Shape intensity of the jagged outline; valid range is 1 (most) to 5 (least); only valid if JaggedOutline is true

Crops this view using the selected closed sketch profile.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Crop2( _    ByVal JaggedOutline As System.Boolean, _    ByVal NoOutline As System.Boolean, _    ByVal ShapeIntensity As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim JaggedOutline As System.Boolean Dim NoOutline As System.Boolean Dim ShapeIntensity As System.Integer Dim value As System.Integer   value = instance.Crop2(JaggedOutline, NoOutline, ShapeIntensity) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Crop2(     System.bool JaggedOutline,    System.bool NoOutline,    System.int ShapeIntensity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Crop2(  &   System.bool JaggedOutline, &   System.bool NoOutline, &   System.int ShapeIntensity ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*JaggedOutline*
:   True to use a jagged outline, false to not; only valid if NoOutline is false

*NoOutline*
:   True to not show an outline, false to show an outline

*ShapeIntensity*
:   Shape intensity of the jagged outline; valid range is 1 (most) to 5 (least); only valid if JaggedOutline is true

#### Return Value

Crop view status as defined in swCropViewErrors\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::Crop2.

# ![](dotnetimages/collapse.gif)Example

[Crop Drawing View Using Jagged Outline (C#)](Crop_Drawing_View_Using_Jagged_Outline_Example_CSharp.htm)

[Crop Drawing View Using Jagged Outline (VB.NET)](Crop_Drawing_View_Using_Jagged_Outline_Example_VBNET.htm)

[Crop Drawing View Using Jagged Outline (VBA)](Crop_Drawing_View_Using_Jagged_Outline_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IsCropped Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsCropped.html)

[IView::CropViewJaggedOutline Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~CropViewJaggedOutline.html)

[IView::CropViewJaggedShapeIntensity Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~CropViewJaggedShapeIntensity.html)

[IView::CropViewNoOutline Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~CropViewNoOutline.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0