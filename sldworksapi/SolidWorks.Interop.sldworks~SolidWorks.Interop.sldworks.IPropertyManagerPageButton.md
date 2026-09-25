<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageButton.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPropertyManagerPageButton Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageButton_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPropertyManagerPageButton Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to access a [PropertyManager page](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2.html) button control.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPropertyManagerPageButton ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageButton ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPropertyManagerPageButton ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPropertyManagerPageButton ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageButton.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Users can resize PropertyManager pages horizontally in SOLIDWORKS 2006 and later. This change in functionality affects the appearance of the buttons on PropertyManager pages created in SOLIDWORKS 2005 and earlier.

In SOLIDWORKS 2005 and earlier, buttons remained aligned vertically at an indented position when a user resized a PropertyManager page. In most instances, these buttons are now centered when a user resizes a PropertyManager page. However, if a button on a PropertyManager page was aligned at the very left edge of the page and it was the only button on that line, then it is assumed that it was intentionally placed at that position and it will stay at that position if a user resizes the page. Any text on the button will also be left justified inside the button. If a button has a bitmap as its label, then the button remains next to the label instead of being centered.

See Using PropertyManagerPage2 and the Related Objects for more information.

# ![](dotnetimages/collapse.gif)Accessors

[IPropertyManagerPage2::AddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~AddControl.html) and [IPropertyManagerPage2::IAddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~IAddControl.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[PropertyManagerPageButton](SWObjectModel.pdf#PropertyManagerPageButton)

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageButton Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageButton_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)