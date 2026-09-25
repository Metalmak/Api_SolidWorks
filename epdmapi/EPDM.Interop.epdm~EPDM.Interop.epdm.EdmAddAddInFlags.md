<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddAddInFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmAddAddInFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddAddInFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for adding add-ins. Used by [IEdmAddInMgr5::AddAddIns](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5~AddAddIns.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmAddAddInFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmAddAddInFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmAddAddInFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmAddin\_AddAllFilesToOneAddIn** | 1 = Add all of the files passed to IEdmAddInMgr5::AddAddIns to the same add-in; this is useful for creating an add-in that has both a 64-bit DLL and a 32-bit DLL |
| **EdmAddin\_Nothing** | 0 = Attempt to create one add-in per file that is passed to IEdmAddInMgr5::AddAddIns |
| **EdmAddin\_ReplaceDuplicates** | 2 = Replace an existing add-in that has the same COM class ID (CLSID) and package name; IEdmAddInMgr5::AddAddIns returns an error if the existing add-in has the same CLSID but a different package name |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)