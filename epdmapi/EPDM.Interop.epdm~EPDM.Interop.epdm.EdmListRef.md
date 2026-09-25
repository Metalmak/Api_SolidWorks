<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRef.html -->

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

| EdmListRef Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRef_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListRef Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about file references.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmListRef     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmListRef : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmListRef : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

```
struct EdmListRef
{
  integer mlChildID;
  integer mlChildFolderID;
  integer mlChildRefVersion;
  integer mlParentFileID;
  integer mlParentFolderID;};
```

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmBatchListing3::GetReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3~GetReferences.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListRef Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListRef_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2014