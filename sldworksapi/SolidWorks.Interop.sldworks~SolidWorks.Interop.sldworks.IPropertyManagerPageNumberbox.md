<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPropertyManagerPageNumberbox Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPropertyManagerPageNumberbox Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to access a [PropertyManager page](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2.html) number box control.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPropertyManagerPageNumberbox ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageNumberbox ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPropertyManagerPageNumberbox ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPropertyManagerPageNumberbox ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageNumberbox.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Cut Body in Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If you implement a... | Then... |
| Spin box | an edit box with attached up and down arrow buttons for incrementing and decrementing the value is created. |
| Combo box/spin box | a text box with:   * a down-arrow button to display the attached drop-down list. You must set up and control the attached drop-down list * up and down buttons for incrementing and decrementing the value   is created.  Use [IPropertyManagerPageNumberbox::Style](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageNumberbox~Style.html) to select the type of combo-box/spin-box number box you want to implement. |

For both types of number boxes, SOLIDWORKS automatically validates the values and units. The up and down arrow buttons automatically increment and decrement the value. Both types of number boxes:

* Accept numerical expressions.

  * Store all values as meters or radians and display them in the units specified in the current unit settings.

NOTE: When a document's unit system is set to a non-metric setting, the dimension precision value (the number of digits displayed after a decimal point) is based on the number of digits specified. It is not based on the document's dimension precision settings.

See Using PropertyManagerPage2 and the Related Objects for more information.

# ![](dotnetimages/collapse.gif)Accessors

[IPropertyManagerPage2::AddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~AddControl.html) and [IPropertyManagerPage2::IAddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~IAddControl.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[PropertyManagerPageNumberbox](SWObjectModel.pdf#PropertyManagerPageNumberbox)

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageNumberbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageNumberbox_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)