<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell~IsLocked.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IsLocked Method (IEdmBomCell) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomCell Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html) : IsLocked Method (IEdmBomCell) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether the file associated with this BOM cell is checked out and can be edited.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function IsLocked() As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsLocked() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsLocked(); ``` | |

#### Return Value

True if the file associated with this BOM cell is available for editing, false if not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomCell](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomCell Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell.html)

[IEdmBomCell Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomCell_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009