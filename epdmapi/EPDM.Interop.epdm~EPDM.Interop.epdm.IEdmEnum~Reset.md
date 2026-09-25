<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~Reset.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Reset Method (IEdmEnum) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html) : Reset Method (IEdmEnum) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Resets the enumerator's cursor to the position before the first element in the list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Reset() ``` | |

| C# |  |
| --- | --- |
| ``` void Reset() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Reset(); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must call [IEdmEnum::MoveNext](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~MoveNext.html) before you can call [IEdmEnum::Current](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~Current.html) to get the first element in the list.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html)

[IEdmEnum Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013