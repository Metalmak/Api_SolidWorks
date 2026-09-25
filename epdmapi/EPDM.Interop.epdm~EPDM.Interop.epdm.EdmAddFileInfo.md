<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo.html -->

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

| EdmAddFileInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddFileInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmAddFileInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmAddFileInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmAddFileInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmAddFileInfo{
  integer [mlSrcDocumentID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mlSrcDocumentID.html);
  integer [mlSrcProjectID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mlSrcProjectID.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mbsPath.html);
  string [mbsNewName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mbsNewName.html);
  integer [mlEdmAddFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mlEdmAddFlags.html);
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo~mlFileID.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmFolder6::AddFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6~AddFiles.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmAddFileInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFileInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.0 of SOLIDWORKS PDM Professional