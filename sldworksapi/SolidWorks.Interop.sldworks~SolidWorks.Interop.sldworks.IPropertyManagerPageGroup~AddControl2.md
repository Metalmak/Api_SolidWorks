<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup~AddControl2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddControl2 Method (IPropertyManagerPageGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup.html) : AddControl2 Method (IPropertyManagerPageGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ID*
:   Resource ID of the control

*ControlType*
:   Type of control as defined in swPropertyManagerPageControlType\_e

*Caption*
:   Caption of the control

*LeftAlign*
:   Left alignment of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e (see **Remarks**)

*Tip*
:   ToolTip text for the control

Adds a control to this PropertyManager page group box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddControl2( _    ByVal ID As System.Integer, _    ByVal ControlType As System.Short, _    ByVal Caption As System.String, _    ByVal LeftAlign As System.Short, _    ByVal Options As System.Integer, _    ByVal Tip As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageGroup Dim ID As System.Integer Dim ControlType As System.Short Dim Caption As System.String Dim LeftAlign As System.Short Dim Options As System.Integer Dim Tip As System.String Dim value As System.Object   value = instance.AddControl2(ID, ControlType, Caption, LeftAlign, Options, Tip) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddControl2(     System.int ID,    System.short ControlType,    System.string Caption,    System.short LeftAlign,    System.int Options,    System.string Tip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddControl2(  &   System.int ID, &   System.short ControlType, &   System.String^ Caption, &   System.short LeftAlign, &   System.int Options, &   System.String^ Tip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ID*
:   Resource ID of the control

*ControlType*
:   Type of control as defined in swPropertyManagerPageControlType\_e

*Caption*
:   Caption of the control

*LeftAlign*
:   Left alignment of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e (see **Remarks**)

*Tip*
:   ToolTip text for the control

#### Return Value

Newly created [control for this PropertyManager page group box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageControl.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageGroup::AddControl2.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPageGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Cut Body in Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method to set properties on the PropertyManager page before it is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IPropertyManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html).

When you specify swAddControlOptions\_e.swControlOptions\_SmallGapAbove for the Options parameter, the gap created between a new control and the previous control is smaller than the typical gap. Also, the control is hidden unless you specify swAddControlOptions\_e.swControlOptions\_Visible for the Options parameter. In the previous versions of this method, IPropertyManagerPageGroup::AddControl and IPropertyManagerGroup::IAddControl, the control was visible regardless if the Options parameter was set or not set to swAddControlOptions\_e.swControlOptions\_Visible.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup.html)

[IPropertyManagerPageGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 SP1, Revision Number 22.1