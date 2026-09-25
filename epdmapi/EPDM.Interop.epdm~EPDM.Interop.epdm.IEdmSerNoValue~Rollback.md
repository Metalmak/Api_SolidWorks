<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue~Rollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback Method (IEdmSerNoValue) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSerNoValue Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue.html) : Rollback Method (IEdmSerNoValue) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Returns the allocated serial number to the serial number generator, so it can be allocated in the future.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback() ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback(); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This method allows you to return generated numbers that you can not use. This helps to avoid gaps between serial numbers.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSerNoValue Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue.html)

[IEdmSerNoValue Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4