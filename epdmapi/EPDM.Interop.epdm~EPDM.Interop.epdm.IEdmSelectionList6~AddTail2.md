<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~AddTail2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddTail2 Method (IEdmSelectionList6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSelectionList6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html) : AddTail2 Method (IEdmSelectionList6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poObject*
:   [EdmSelectionObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject.html) structure; describes the object to add to the end of the list

Adds an item to the end of this list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddTail2( _    ByRef poObject As EdmSelectionObject _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddTail2(     ref EdmSelectionObject poObject ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddTail2(  &   EdmSelectionObject% poObject ) ``` | |

#### Parameters

*poObject*
:   [EdmSelectionObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject.html) structure; describes the object to add to the end of the list

# ![](dotnetimages/collapse.gif)Example

[Display Menu of Commands (VB.NET)](Display_Menu_of_Commands_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSelectionList6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html)

[IEdmSelectionList6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010