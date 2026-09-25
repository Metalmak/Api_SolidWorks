<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6~OnTabClicked.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnTabClicked Method (IPropertyManagerPage2Handler6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html) : OnTabClicked Method (IPropertyManagerPage2Handler6) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the tab clicked (see Remarks)

Obsoleted. Superseded by [IPropertyManagerPage2Handler7::OnTabClicked](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler7~OnTabClicked.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnTabClicked( _    ByVal Id As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler6 Dim Id As System.Integer Dim value As System.Boolean   value = instance.OnTabClicked(Id) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnTabClicked(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnTabClicked(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   ID of the tab clicked (see Remarks)

#### Return Value

True if the tab clicked is processed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler6::OnTabClicked.

# ![](dotnetimages/collapse.gif)Remarks

The value of Id is the ID that was specified when the tab was created by IPropertyManagerPage2::AddTab.

When a user clicks a tab, control is passed to the add-in via this method. The add-in is expected to show or hide groups and controls intended to be visible or hidden on that tab.

Your add-in is responsible for showing and hiding the controls on a tab to simulate moving between tabs, making it look like the tab is a container for the controls. However, tabs are not containers for the groups or controls. Tabs are controls that are displayed in a certain way, making them look like control containers.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler6 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6.html)

[IPropertyManagerPage2Handler6 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0