<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox~DisplayedUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DisplayedUnit Property (IPropertyManagerPageNumberbox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageNumberbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox.html) : DisplayedUnit Property (IPropertyManagerPageNumberbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the unit type to display in this PropertyManager page number box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DisplayedUnit As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageNumberbox Dim value As System.Integer   instance.DisplayedUnit = value   value = instance.DisplayedUnit ``` | |

| C# |  |
| --- | --- |
| ``` System.int DisplayedUnit {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DisplayedUnit {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Unit type to display in this PropertyManager page number box (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageNumberbox::DisplayedUnit.

# ![](dotnetimages/collapse.gif)Remarks

This property depends on the unit type specified for the [IPropertyManagerPageNumberbox::SetRange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageNumberbox~SetRange2.html)'s Units parameter, which is a value from swNumberboxUnitType\_e.

|  |  |
| --- | --- |
| **If IPropertyManagerPageNumberbox::SetRange2's Units parameter is...** | **Then specifiy an enumerator from this enumeration for IPropertyManagerPageNumber::DisplayedUnit...** |
| swNumberBox\_Length | swLengthUnit\_e |
| swNumberBox\_Angle | swAngleUnit\_e |
| swNumberBox\_Force | swUnitsForce\_e |
| swNumberBox\_Time | swUnitsTimeUnit\_e |

For example, IPropertyManagerPageNumberbox::DisplayedUnit allows an add-in to have a number box that shows length values in inches, even though the system default units are meters. Remember that the values specified for both [IPropertyManagerPageNumberbox::Value](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageNumberbox~Value.html) and IPropertyManagerPageNumberbox::SetRange2 are in system units; IPropertyManagerPageNumberbox::DisplayedUnits simply controls how that value is displayed in the PropertyManager page number box.

You can call IPropertyManagerPageNumberbox::DisplayedUnit and change the units displayed in a number box while a Propertymanager page is displayed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageNumberbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox.html)

[IPropertyManagerPageNumberbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox_members.html)