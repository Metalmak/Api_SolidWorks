<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~FullName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FullName Property (IDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html) : FullName Property (IDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the full name of a dimension including the feature and the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property FullName As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimension Dim value As System.String   value = instance.FullName ``` | |

| C# |  |
| --- | --- |
| ``` System.string FullName {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ FullName {    System.String^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Name of the dimension including the feature and model

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Dimension::FullName.

# ![](dotnetimages/collapse.gif)Example

[Determine if Display Dimension Marked for Drawing (VBA)](Determine_if_Display_Dimension_Marked_for_Drawing_Example_VB.htm)

[Get Block Information (VBA)](Get_Block_Information_Example_VB.htm)

[Get Dimension Values in All Configurations (VBA)](Get_Dimension_Values_in_All_Configurations_Example_VB.htm)

[Get Mate Definition (VBA)](Get_Mate_Definition_Example_VB.htm)

[Iterate Through Dimensions in Model (VBA)](Iterate_Through_Dimensions_in_Model_Example_VB.htm)

[Set Dimensions to Mid-tolerance (VBA)](Set_Dimensions_to_Mid-Tolerance_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The syntax of the name returned is:

<Dimension Name>@<Feature Name>@<Model>

where:

* <Dimension Name> is the name of the dimension as returned from [IDimension::Name](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~Name.html)

  * <Feature Name> is the name of the feature that the dimension is on

    * <Model> is the name of the model containing the feature

For example:

"D1@Sketch1@Part4.Part"

# ![](dotnetimages/collapse.gif)See Also

####

[IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html)

[IDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension_members.html)