<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6~OnComboboxSelectionChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnComboboxSelectionChanged Method (IPropertyManagerPage2Handler6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html) : OnComboboxSelectionChanged Method (IPropertyManagerPage2Handler6) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the combo box

*Item*
:   ID of the item

Obsoleted. Superseded by [IPropertyManagerPage2Handler7::OnComboboxSelectionChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler7~OnComboboxSelectionChanged.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnComboboxSelectionChanged( _    ByVal Id As System.Integer, _    ByVal Item As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler6 Dim Id As System.Integer Dim Item As System.Integer   instance.OnComboboxSelectionChanged(Id, Item) ``` | |

| C# |  |
| --- | --- |
| ``` void OnComboboxSelectionChanged(     System.int Id,    System.int Item ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnComboboxSelectionChanged(  &   System.int Id, &   System.int Item ) ``` | |

#### Parameters

*Id*
:   ID of the combo box

*Item*
:   ID of the item

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler6::OnComboboxSelectionChanged.

# ![](dotnetimages/collapse.gif)Remarks

If the user can edit the text in the text box, then use this method with [IPropertyManagerPage2Handler6::OnComboxEditChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler6~OnComboboxEditChanged.html) to  find out what is in the text box of the combo box.

When this method is called, the control may not yet be updated with the current selection, so the IPropertyManagerPageCombobox::CurrentSelection property is not reliable. To get the current text, use the value of Item that is passed into the method as the argument to IPropertyManagerPageCombobox::ItemText.

If the user has edited the text in the text box and then clicks the arrow to show or hide the list box of the combo box, and the text in the text box matches the first character in any of the items in the list, then that item is automatically selected in the list and this method is called, indicating that the selected item has changed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html)

[IPropertyManagerPage2Handler6 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0