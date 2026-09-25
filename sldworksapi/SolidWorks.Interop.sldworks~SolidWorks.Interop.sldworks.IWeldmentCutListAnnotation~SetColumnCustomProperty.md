<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListAnnotation~SetColumnCustomProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetColumnCustomProperty Method (IWeldmentCutListAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWeldmentCutListAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListAnnotation.html) : SetColumnCustomProperty Method (IWeldmentCutListAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Column for which to get the custom property

*CustomProp*
:   Custom property for this user-defined column

Sets the custom property of the specified user-defined column.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetColumnCustomProperty( _    ByVal Index As System.Integer, _    ByVal CustomProp As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWeldmentCutListAnnotation Dim Index As System.Integer Dim CustomProp As System.String Dim value As System.Boolean   value = instance.SetColumnCustomProperty(Index, CustomProp) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetColumnCustomProperty(     System.int Index,    System.string CustomProp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetColumnCustomProperty(  &   System.int Index, &   System.String^ CustomProp ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Column for which to get the custom property

*CustomProp*
:   Custom property for this user-defined column

#### Return Value

True if the custom property is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WeldmentCutListAnnotation::SetColumnCustomProperty.

# ![](dotnetimages/collapse.gif)Remarks

Use this method to create a user-defined column where each row in the column is automatically filled in with the custom property value for that particular configuration. The default title for the column is the name of the custom property. If the specified custom property is not a valid custom property, then each row in the column remains empty.

To create a user-defined column that is not attached to a custom property; for example, you want to fill in each row of the column yourself, use this method with the CustomProp value specified as the title of the column.

To get the list of available custom properties, use [IWeldmentCutListAnnotation::GetAllCustomProperties](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldmentCutListAnnotation~GetAllCustomProperties.html) or [IWeldmentCustListAnnotation::IGetAllCustomProperties](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldmentCutListAnnotation~IGetAllCustomProperties.html). The list of available custom properties includes all of the items in the weldment cut-list table, which includes items from the file summary items and file custom properties that have been set.

This method returns false if the column is not a user-defined column, and no action is taken.

# ![](dotnetimages/collapse.gif)See Also

####

[IWeldmentCutListAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListAnnotation.html)

[IWeldmentCutListAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListAnnotation_members.html)

[IWeldmentCutListAnnotation::GetColumnCustomProperty Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListAnnotation~GetColumnCustomProperty.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0