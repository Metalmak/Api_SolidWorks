<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle~SetStyle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetStyle Method (IDetailCircle) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDetailCircle Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle.html) : SetStyle Method (IDetailCircle) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Style as defined by swDetViewStyle\_e

Sets the style of the detail circle (for example, standard, broken, leader, no leader, or connected).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetStyle( _    ByVal Style As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDetailCircle Dim Style As System.Integer Dim value As System.Boolean   value = instance.SetStyle(Style) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetStyle(     System.int Style ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetStyle(  &   System.int Style ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Style as defined by swDetViewStyle\_e

#### Return Value

True if setting the detail view style is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DetailCircle::SetStyle.

# ![](dotnetimages/collapse.gif)Remarks

This method sets different styles for the detail view display, following the detailing standard, as a broken circle, as a circle or profile with or without a leader to the detail label, or with a line connecting the detail circle or profile with the detail view.

This method automatically load the model for the detail view, if necessary, without prompting the user.

If the style of the detail circle is swDetViewBROKEN or swDetViewSTANDARD and the current detailing standard is ANSI, then this method automatically switches the detail circle or profile display to circle because a broken circle style requires a circle, not a profile.

# ![](dotnetimages/collapse.gif)See Also

####

[IDetailCircle Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle.html)

[IDetailCircle Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle_members.html)

[IDetailCircle::GetStyle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle~GetStyle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP1, Revision Number 12.1