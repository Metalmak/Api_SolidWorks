<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSearchToken.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmSearchToken Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmSearchToken Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Values that determine which search criteria to set.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmSearchToken     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmSearchToken : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmSearchToken : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmstok\_AllVersions** | 2 = VT\_BOOL; search all versions of a file |
| **Edmstok\_ContentText** | 36 = VT\_BSTR; search for this string in the file body itself; this requires that the indexing service has been enabled in the administration tool |
| **Edmstok\_ContentTextExact** | 40 = VT\_BOOL; find only exact matches of the content string, not individual words |
| **Edmstok\_ContentTextInBody** | 37 = VT\_BOOL; do content search in the file body |
| **Edmstok\_ContentTextInProperties** | 38 = VT\_BOOL; do content search in the file custom properties |
| **Edmstok\_ContentTextOr** | 39 = VT\_BOOL; search for any words, instead of all of the words, in the content search string |
| **Edmstok\_FindFiles** | 31 = VT\_BOOL; return files in the result |
| **Edmstok\_FindFolders** | 32 = VT\_BOOL; return folders in the result |
| **Edmstok\_FindItems** | 41 = VT\_BOOL; return items in the search result |
| **Edmstok\_FolderID** | 5 = VT\_I4; ID of folder to start the search in |
| **Edmstok\_HistoryAfter** | 34 = VT\_DATE; search history after this date |
| **Edmstok\_HistoryBefore** | 33 = VT\_DATE; search history before this date |
| **Edmstok\_HistoryString** | 25 = VT\_BSTR; search for string in file history |
| **Edmstok\_HistoryStringConfiguration** | 43 = VT\_BOOL; search for keyword among configuration names |
| **Edmstok\_HistoryStringFileName** | 42 = VT\_BOOL; search for keyword among file names |
| **Edmstok\_HistoryStringLabels** | 27 = VT\_BOOL; search labels for the history string |
| **Edmstok\_HistoryStringRevisionComment** | 29 = VT\_BOOL; search revisions comments for the history string |
| **Edmstok\_HistoryStringStateComment** | 28 = VT\_BOOL; search workflow state change comments for the history string |
| **Edmstok\_HistoryStringVariableValues** | 30 = VT\_BOOL; search variable values for the history string |
| **Edmstok\_HistoryStringVersionComment** | 26 = VT\_BOOL; search version comments for the history string |
| **Edmstok\_Label** | 20 = VT\_BSTR; search for this string in labels |
| **Edmstok\_LabelAfter** | 24 = VT\_DATE; search for labels set after this date |
| **Edmstok\_LabelBefore** | 23 = VT\_DATE; search for labels set before this date |
| **Edmstok\_LabelByUser** | 22 = VT\_BSTR; search for files where a user with this name created a label |
| **Edmstok\_LabelComment** | 21 = VT\_BOOL; search for the label string in the comment |
| **Edmstok\_Locked** | 6 = VT\_BOOL; return checked out files? |
| **Edmstok\_LockedBy** | 8 = VT\_BSTR; search for files checked out by users with this name |
| **Edmstok\_Name** | 3 = VT\_BSTR; name of file or folder for which to search |
| **Edmstok\_Recursive** | 1 = VT\_BOOL; search subfolders recursively |
| **Edmstok\_StateAfter** | 19 = VT\_DATE; only find files where a state change was made after this date |
| **Edmstok\_StateBefore** | 18 = VT\_DATE; only find files where a state change was made before this date |
| **Edmstok\_StateByUser** | 17 = VT\_BSTR; find files where a user with this name has changed workflow state |
| **Edmstok\_StateHistoric** | 16 = VT\_BOOL; search in historic states, not just the latest state |
| **Edmstok\_StateID** | 15 = VT\_I4; only find files in the workflow state with this ID |
| **Edmstok\_StateName** | 14 = VT\_BSTR; only find files in workflow states with this name |
| **Edmstok\_Unlocked** | 7 = VT\_BOOL; return checked in files? |
| **Edmstok\_VersionComment** | 10 = VT\_BSTR; search for files with this version comment |
| **Edmstok\_VersionsAfter** | 13 = VT\_DATE; only find files that have been checked in after this date |
| **Edmstok\_VersionsBefore** | 12 = VT\_DATE; only find files that have been checked in before this date |
| **Edmstok\_VersionsByUser** | 11 = VT-BSTR; only find files that have been checked in by a user with this name |
| **Edmstok\_WorkflowName** | 35 = VT\_BSTR; search for files part of this workflow |

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmSearch6::GetToken](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6~GetToken.html) and [IEdmSearch6::SetToken](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6~SetToken.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)