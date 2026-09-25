<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo.html -->

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

| EdmObjectInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmObjectInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Use in calls to [IEdmVault9::GetObjects](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9~GetObjects.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmObjectInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmObjectInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmObjectInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmObjectInfo

{
  [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html) [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo~meType.html);
  object [moObjectID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo~moObjectID.html);
  [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html)\*  [mpoObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo~mpoObject.html);
  integer [mhResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo~mhResult.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Update Card Variables (C#)](Batch_Update_Variables_Example_CSharp.htm)

[Batch Update Card Variables (VB.NET)](Batch_Update_Variables_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The structure contains both input and output.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmObjectInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008