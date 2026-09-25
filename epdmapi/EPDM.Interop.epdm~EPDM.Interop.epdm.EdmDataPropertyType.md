<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDataPropertyType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmDataPropertyType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmDataPropertyType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Property types; used in calls to [IEdmData::Get](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Get.html) and [IEdmData::Set](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Set.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmDataPropertyType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmDataPropertyType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmDataPropertyType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmProp\_ID** | 1 = Database ID |
| **EdmProp\_LinkPath** | 8 = Path to linked file |
| **EdmProp\_Name** | 4 = Name of a file, folder, variable, etc. |
| **EdmProp\_Nothing** | 0 = Invalid property |
| **EdmProp\_Object** | 3 = [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html) |
| **EdmProp\_ObjectType** | 2 = [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) |
| **EdmProp\_Path** | 5 = File or folder path |
| **EdmProp\_Value** | 6 = Variable value |
| **EdmProp\_Vault** | 7 = [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)