<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5~GetHeadPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetHeadPosition Method (IEdmStrLst5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmStrLst5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) : GetHeadPosition Method (IEdmStrLst5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the strings in this list.

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

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position in the list of the first string (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first string to [IEdmStrLst5::GetNext](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5~GetNext.html) to get the first string in this list. Then call IEdmStrLst5::GetNext repeatedly to get the rest of the strings in this list.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmStrLst5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html)

[IEdmStrLst5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2