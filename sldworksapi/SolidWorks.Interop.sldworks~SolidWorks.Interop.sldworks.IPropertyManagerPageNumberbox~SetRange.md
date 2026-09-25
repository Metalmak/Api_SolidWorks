<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox~SetRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetRange Method (IPropertyManagerPageNumberbox) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageNumberbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox.html) : SetRange Method (IPropertyManagerPageNumberbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Units*
:   Number box units as defined in swNumberboxUnitType\_e

*Minimum*
:   Number box minimum value

*Maximum*
:   Number box maximum value

*Increment*
:   Number box increment

*Inclusive*
:   True sets the range as inclusive, false sets it as exclusive

Obsolete. Superseded by [PropertyManagerPageNumberbox::SetRange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageNumberbox~SetRange2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRange( _    ByVal Units As System.Integer, _    ByVal Minimum As System.Double, _    ByVal Maximum As System.Double, _    ByVal Increment As System.Double, _    ByVal Inclusive As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageNumberbox Dim Units As System.Integer Dim Minimum As System.Double Dim Maximum As System.Double Dim Increment As System.Double Dim Inclusive As System.Boolean   instance.SetRange(Units, Minimum, Maximum, Increment, Inclusive) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRange(     System.int Units,    System.double Minimum,    System.double Maximum,    System.double Increment,    System.bool Inclusive ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRange(  &   System.int Units, &   System.double Minimum, &   System.double Maximum, &   System.double Increment, &   System.bool Inclusive ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Units*
:   Number box units as defined in swNumberboxUnitType\_e

*Minimum*
:   Number box minimum value

*Maximum*
:   Number box maximum value

*Increment*
:   Number box increment

*Inclusive*
:   True sets the range as inclusive, false sets it as exclusive

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageNumberbox::SetRange.

# ![](dotnetimages/collapse.gif)Example

[Cut Body in Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method to set properties on the PropertyManager page before it is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IProperytManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageNumberbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox.html)

[IPropertyManagerPageNumberbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0