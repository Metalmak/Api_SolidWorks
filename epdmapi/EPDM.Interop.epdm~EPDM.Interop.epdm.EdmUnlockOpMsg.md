<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockOpMsg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUnlockOpMsg Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUnlockOpMsg Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of constant passed to [IEdmUnlockOpCallback::MsgBox](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback~MsgBox.html) when the caller should either display a message to the user or process the message in some other way.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUnlockOpMsg     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUnlockOpMsg : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUnlockOpMsg : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Euom\_AdminUndoLock** | 5 = You are logged in as Admin and are trying to undo the check-out flag on a file checked out by another user |
| **Euom\_AdminUnlock** | 8 = You are logged in as Admin and are trying to check in a file that is checked out by another user |
| **Euom\_CircularReference** | 9 = The files checked have circular references |
| **Euom\_DocumentDoesNotMeetConditionsInAnyCategory** | 11 = The document cannot be unlocked because it does not meet the conditions of any category |
| **Euom\_DocumentDoesNotMeetConditionsInAnyWorkflow** | 10 = The document cannot be unlocked because it does not meet the conditions of any workflow |
| **Euom\_DuplicateUniqueVar** | 1 = The file has a unique variable with a duplicate value |
| **Euom\_LocalFileNotFound** | 6 = The local copy of the file was not found |
| **Euom\_LocalFileShareError** | 7 = Sharing violation accessing the local copy of the file |
| **Euom\_MissingMandatoryVar** | 2 = The file cannot be checked in, because the file contains a unique and constrained variable with a value that is already used elsewhere |
| **Euom\_UndoLockModified** | 4 = The file about whose check out you about to undo, has been modified |
| **Euom\_UnknownFileFormat** | 3 = SOLIDWORKS PDM Professional cannot read references or variables from the file, because its file format is unknown |

# ![](dotnetimages/collapse.gif)Remarks

This constant tells which message to display.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)