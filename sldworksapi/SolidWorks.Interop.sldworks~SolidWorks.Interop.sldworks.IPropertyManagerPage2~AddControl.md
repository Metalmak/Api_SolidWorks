<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2~AddControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddControl Method (IPropertyManagerPage2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) : AddControl Method (IPropertyManagerPage2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ID*
:   Resource ID of this control; API passes this user-defined value back to the add-in through the IPropertyManagerPage2Handler8 interface

*ControlType*
:   Type of control as defined in swPropertyManagerPageControlType\_e

*Caption*
:   Caption of this control

*LeftAlign*
:   Left-align property of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e

*Tip*
:   ToolTip for this control

Obsolete. Superseded by [IPropertyManagerPage2::AddControl2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~AddControl2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddControl( _    ByVal ID As System.Integer, _    ByVal ControlType As System.Short, _    ByVal Caption As System.String, _    ByVal LeftAlign As System.Short, _    ByVal Options As System.Integer, _    ByVal Tip As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2 Dim ID As System.Integer Dim ControlType As System.Short Dim Caption As System.String Dim LeftAlign As System.Short Dim Options As System.Integer Dim Tip As System.String Dim value As System.Object   value = instance.AddControl(ID, ControlType, Caption, LeftAlign, Options, Tip) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddControl(     System.int ID,    System.short ControlType,    System.string Caption,    System.short LeftAlign,    System.int Options,    System.string Tip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddControl(  &   System.int ID, &   System.short ControlType, &   System.String^ Caption, &   System.short LeftAlign, &   System.int Options, &   System.String^ Tip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ID*
:   Resource ID of this control; API passes this user-defined value back to the add-in through the IPropertyManagerPage2Handler8 interface

*ControlType*
:   Type of control as defined in swPropertyManagerPageControlType\_e

*Caption*
:   Caption of this control

*LeftAlign*
:   Left-align property of this control as defined in swPropertyManagerPageControlLeftAlign\_e

*Options*
:   Options as defined in swAddControlOptions\_e

*Tip*
:   ToolTip for this control

#### Return Value

Newly created [PropertyManager page control](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageControl.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2::AddControl.

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method to set properties on the PropertyManager before the page is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IPropertyManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html).

To follow the SOLIDWORKS standards when designing a new PropertyManager page, it is a good idea to use [IPropertyManagerPage2::AddGroupBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~AddGroupBox.html) or [IPropertyManagerPage2::IAddGroupBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~IAddGroupBox.html) and IPropertyManagerPageGroup::AddControl or [IPropertyManagerPageGroup::IAddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~IAddControl.html) to add controls for the page inside group boxes.

When you specify swControlOptions\_SmallGapAbove for the Options parameter, a gap, smaller than the typical gap, is used between a new control and the previous control.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html)

[IPropertyManagerPage2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0