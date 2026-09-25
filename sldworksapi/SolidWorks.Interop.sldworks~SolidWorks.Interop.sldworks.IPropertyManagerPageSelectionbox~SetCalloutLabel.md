<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox~SetCalloutLabel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetCalloutLabel Method (IPropertyManagerPageSelectionbox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html) : SetCalloutLabel Method (IPropertyManagerPageSelectionbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Label*
:   Default callout label

Sets the default callout label for selections made in this selection box on the PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCalloutLabel( _    ByVal Label As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageSelectionbox Dim Label As System.String Dim value As System.Boolean   value = instance.SetCalloutLabel(Label) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetCalloutLabel(     System.string Label ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetCalloutLabel(  &   System.String^ Label ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Label*
:   Default callout label

#### Return Value

True if the callout label was set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageSelectionbox::SetCalloutLabel.

# ![](dotnetimages/collapse.gif)Remarks

This property can be used at any time, whether or not the callout is displayed. The label must not be an empty string. By default, the selection box is created without callouts for selections. This method overrides that behavior.

For more control, you can implement the IPropertyManagerPage2Handler5::OnSelectionboxCalloutCreated property, which allows you to collect information such as the selection type from the last selection. Next, use the [IPropertyManagerPageSelectionbox::Callout](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageSelectionbox~Callout.html) property to get the [ICallout](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout.html) object. Then, use that object's various properties to control the callout text and display characteristics based on that selection information.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html)

[IPropertyManagerPageSelectionbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0