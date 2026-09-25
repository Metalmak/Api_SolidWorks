<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup~IAddControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddControl Method (IPropertyManagerPageGroup) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup.html) : IAddControl Method (IPropertyManagerPageGroup) |

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
:   Left align property of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e

*Tip*
:   ToolTip text for the control

Obsolete. Superseded by [IPropertyManagerPageGroup::AddControl2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageGroup~AddControl2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddControl( _    ByVal ID As System.Integer, _    ByVal ControlType As System.Short, _    ByVal Caption As System.String, _    ByVal LeftAlign As System.Short, _    ByVal Options As System.Integer, _    ByVal Tip As System.String _ ) As PropertyManagerPageControl ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageGroup Dim ID As System.Integer Dim ControlType As System.Short Dim Caption As System.String Dim LeftAlign As System.Short Dim Options As System.Integer Dim Tip As System.String Dim value As PropertyManagerPageControl   value = instance.IAddControl(ID, ControlType, Caption, LeftAlign, Options, Tip) ``` | |

| C# |  |
| --- | --- |
| ``` PropertyManagerPageControl IAddControl(     System.int ID,    System.short ControlType,    System.string Caption,    System.short LeftAlign,    System.int Options,    System.string Tip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` PropertyManagerPageControl^ IAddControl(  &   System.int ID, &   System.short ControlType, &   System.String^ Caption, &   System.short LeftAlign, &   System.int Options, &   System.String^ Tip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ID*
:   Resource ID of the control

*ControlType*
:   Type of control as defined in swPropertyManagerPageControlType\_e

*Caption*
:   Caption of the control

*LeftAlign*
:   Left align property of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e

*Tip*
:   ToolTip text for the control

#### Return Value

Newly created [control for this PropertyManager page group box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageControl.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageGroup::IAddControl.

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method to set properties on the PropertyManager page before it is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IPropertyManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html).

When you specify swControlOptions\_SmallGapAbove for the Options parameter, gap is used between a new control and the previous control that is smaller than the typical gap.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup.html)

[IPropertyManagerPageGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup_members.html)

[IPropertyManagerPageGroup::AddControl Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageGroup~AddControl.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0