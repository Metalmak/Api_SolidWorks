<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~MoveNext.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| MoveNext Method (IEdmEnum) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html) : MoveNext Method (IEdmEnum) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Forwards the enumeration cursor to the next element in the list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function MoveNext() As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MoveNext() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MoveNext(); ``` | |

#### Return Value

True if the cursor moved to the next element successfully, false if not

# ![](dotnetimages/collapse.gif)Remarks

This method is used implicitly in the For Each command loops of .NET programs.

After calling this method, call [IEdmEnum::Current](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~Current.html) to access the element currently pointed to by the enumerator's cursor.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html)

[IEdmEnum Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013