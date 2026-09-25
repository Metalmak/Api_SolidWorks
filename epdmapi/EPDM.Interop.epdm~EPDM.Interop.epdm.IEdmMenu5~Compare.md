<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~Compare.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Compare Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : Compare Method (IEdmMenu5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poMenu*
:   [Menu](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

Compares this IEdmMenu5 menu with another menu to see if they contain the same menu items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Compare( _    ByVal poMenu As IEdmMenu5 _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Compare(     IEdmMenu5 poMenu ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Compare(  &   IEdmMenu5^ poMenu ) ``` | |

#### Parameters

*poMenu*
:   [Menu](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

#### Return Value

True if the objects are equal, false if not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: Success, but the objects are different (pbEqual returned false).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional