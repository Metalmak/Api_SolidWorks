<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mbsData.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| mbsData Field | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [EdmRevComponent2 Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html) : mbsData Field |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Format string entered in the administration tool if [mlEdmRevComponentFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2~mlEdmRevComponentFlags.html) contains the flag Edmrcf\_TypeFormatString; if mbsDataField contains Edmrcf\_TypeList, then the data member contains a new line-delimited list of list items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public mbsData As System.String ``` | |

| C# |  |
| --- | --- |
| ``` public System.string mbsData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public: System.String^ mbsData ``` | |

# ![](dotnetimages/collapse.gif)Remarks

The mbsData member can contain the following format specifiers when mlEdmRevComponentFlags contains Edmrcf\_TypeFormatString.

|  |  |
| --- | --- |
| **Specifier** | **Meaning** |
| %C | Uppercase A, B, C...Z |
| %c | Lowercase a, b, c...z |
| %01d | Number, 0-padded to 1 digit |
| %02d | Number, 0-padded to 2 digits, etc. |
| %01x | Lowercase hex number, 0-padded to 1 digit |
| %02x | Lowercase hex number, 0-padded to 2 digits, etc. |
| %01X | Uppercase hex number, 0-padded to 1 digit |
| %02X | Uppercase hex number, 0-padded to 2 digits, etc. |
| %4y | 4-digit year |
| %2y | 2-digit year |
| %01m | Month number without 0 padding (1-12) |
| %02m | Month number, 0-padded to two digits (01-12) |
| %01D | Day number without 0 padding (1-31) |
| %02D | Day number, 0-padded to 2 digits (00-31) |
| %01H | Hour without 0 padding (0-23) |
| %02H | Hour, 0-padded to 2 digits (00-23) |
| %01M | Minute without 0 padding (0-59) |
| %02M | Minute, 0-padded to 2 digits (00-59) |
| %01S | Second without 0 padding (0-59) |
| %02S | Second, 0-padded to 2 digits (00-59) |

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRevComponent2 Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html)

[EdmRevComponent2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2_members.html)