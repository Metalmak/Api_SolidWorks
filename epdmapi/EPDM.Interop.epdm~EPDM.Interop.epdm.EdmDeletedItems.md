<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html -->

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

| EdmDeletedItems Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmDeletedItems Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about deleted items.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmDeletedItems     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmDeletedItems : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmDeletedItems : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmDeletedItems

{
  integer [mlFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems~mlFileID.html);
  integer [mlObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems~mlObjectType.html);
  integer [mlProjectID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems~mlProjectID.html);
  string [moName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems~moName.html);
};

# ![](dotnetimages/collapse.gif)See Also

####

[EdmDeletedItems Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Pro 2018