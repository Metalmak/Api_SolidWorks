<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageListbox~SetSelectedItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSelectedItem Method (IPropertyManagerPageListbox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageListbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageListbox.html) : SetSelectedItem Method (IPropertyManagerPageListbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Item*
:   Index of the item to select or clear

*Selected*
:   True to select the item, false to not

Sets whether an item is selected or cleared in a list box enabled for multiple selection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSelectedItem( _    ByVal Item As System.Short, _    ByVal Selected As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageListbox Dim Item As System.Short Dim Selected As System.Boolean Dim value As System.Boolean   value = instance.SetSelectedItem(Item, Selected) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSelectedItem(     System.short Item,    System.bool Selected ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSelectedItem(  &   System.short Item, &   System.bool Selected ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Item*
:   Index of the item to select or clear

*Selected*
:   True to select the item, false to not

#### Return Value

True if the item was selected or cleared, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageListbox::SetSelectedItem.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPageListbox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageListbox.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The value specified for Item must be a valid index number. If it is not, then this method returns false. Thus, set up your list item index before using this method.

If you use this method to set a selected item in a single-selection style list box and another item in the list box is already selected, then that item is automatically cleared. You can use this method to clear a selection in a single-selection style list box, which results in no current selection in that list box.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageListbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageListbox.html)

[IPropertyManagerPageListbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageListbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0