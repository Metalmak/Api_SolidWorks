<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~GetHeadPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetHeadPosition Method (IEdmSelectionList5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html) : GetHeadPosition Method (IEdmSelectionList5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the items in this list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetHeadPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetHeadPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetHeadPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of first element in this list

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSelectionList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the position of the first item to [IEdmSelectionList5::GetNext](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~GetNext.html) to get the first item in this list. Then call IEdmSelectionList5::GetNext repeatedly to get the rest of the items in this list.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSelectionList5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

[IEdmSelectionList5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2