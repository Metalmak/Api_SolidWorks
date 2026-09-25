<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddCallbackMsgID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmAddCallbackMsgID Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddCallbackMsgID Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Message IDs used in the message box during an add operation.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmAddCallbackMsgID     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmAddCallbackMsgID : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmAddCallbackMsgID : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmAddMsg\_ClearUnique** | 2 = Copy over the existing file that has unique values? |
| **EdmAddMsg\_DeleteSource** | 5 = Could not delete a source file during a move operation |
| **EdmAddMsg\_FileFmtReadError** | 4 = File could not be read by the file format plugin |
| **EdmAddMsg\_GenericError** | 0 = Generic error |
| **EdmAddMsg\_MissingPluginComponent** | 3 = File format plugin component is missing |
| **EdmAddMsg\_ReplaceLocal** | 1 = Replace the existing file with the same name? |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)