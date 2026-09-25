<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetSolidHatchCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSolidHatchCount Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetSolidHatchCount Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArraySize*
:   Number of solid-fill hatches

Gets the number of visible solid-fill hatches in a detail, break, or crop view and the size of the array for their boundary data.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSolidHatchCount( _    ByRef ArraySize As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim ArraySize As System.Integer Dim value As System.Integer   value = instance.GetSolidHatchCount(ArraySize) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSolidHatchCount(     out System.int ArraySize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSolidHatchCount(  &   [Out] System.int ArraySize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArraySize*
:   Number of solid-fill hatches

#### Return Value

Size of the array for the solid-fill hatches boundary data

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetSolidHatchCount.

# ![](dotnetimages/collapse.gif)Example

[Get Solid-fill Hatch Information (VB.NET)](Get_Solid-fill_Hatch_Information_Example_VBNET.htm)

[Get Solid-fill Hatch Information (VBA)](Get_Solid-fill_Hatch_Information_Example_VB6.htm)

[Get Solid-fill Hatch Information (C#)](Get_Solid-fill_Hatch_Information_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To get information about solid-fill hatches in drawing views, use [IView::GetFaceHatchCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFaceHatchCount.html), [IView::GetFaceHatches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFaceHatches.html), and [IView::IGetFaceHatches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetFaceHatches.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetSolidHatchInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetSolidHatchInfo.html)

[IView::IGetSolidHatchInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetSolidHatchInfo.html)

[ISketch::GetSketchHatches Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetSketchHatches.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0