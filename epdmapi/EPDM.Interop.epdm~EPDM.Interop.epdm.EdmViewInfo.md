<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo.html -->

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

| EdmViewInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmViewInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a file vault view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmViewInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmViewInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmViewInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmViewInfo{
  string [mbsVaultName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo~mbsVaultName.html);
  string [mbsViewID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo~mbsViewID.html);
  string [mbsVaultID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo~mbsVaultID.html);
  string [mbsPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo~mbsPath.html);
  short [mbLoggedIn](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo~mbLoggedIn.html);
};

# ![](dotnetimages/collapse.gif)Example

[Destroy Deleted Files in Vault (C#)](Destroy_Deleted_Files_in_Vault_Example_CSharp.htm)

[Destroy Deleted Files in Vault (VB.NET)](Destroy_Deleted_Files_in_Vault_Example_VBNET.htm)

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This structure is returned by [IEdmVault8::GetVaultViews](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8~GetVaultViews.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmViewInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmViewInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional