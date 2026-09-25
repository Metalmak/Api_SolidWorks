<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSlider~LineSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LineSize Property (IPropertyManagerPageSlider) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageSlider Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSlider.html) : LineSize Property (IPropertyManagerPageSlider) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets how much the slider moves when the arrow keys are used to move the slider.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LineSize As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageSlider Dim value As System.Integer   instance.LineSize = value   value = instance.LineSize ``` | |

| C# |  |
| --- | --- |
| ``` System.int LineSize {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int LineSize {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

How much the slider moves when arrow keys are used to move the slider

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageSlider::LineSize.

# ![](dotnetimages/collapse.gif)Example

[Set Up PropertyManager Page Slider Control (C++)](Set_Up_PropertyManager_Page_Slider_Control_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you do not set this property, the value defaults to 1.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageSlider Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSlider.html)

[IPropertyManagerPageSlider Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSlider_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0