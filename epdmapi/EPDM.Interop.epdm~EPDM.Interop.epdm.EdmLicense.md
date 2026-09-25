<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense.html -->

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

| EdmLicense Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmLicense Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a license type and is returned by [IEdmVault11::GetLicense](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetLicense.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmLicense     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmLicense : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmLicense : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmLicense

{
  [enum EdmLicenseType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicenseType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense~meType.html);
  integer [mlUserCount](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense~mlUserCount.html);
};

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmLicense Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLicense_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010