<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html -->

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

| EdmRawReference Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRawReference Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a file reference.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRawReference     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRawReference : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRawReference : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRawReference

{
  string [mbsRefID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference~mbsRefID.html);
  string [mbsIncludePath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference~mbsIncludePath.html);
  string [mbsRefName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference~mbsRefName.html);
  integer [mlFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference~mlFlags.html);
  integer [mlCount](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference~mlCount.html);
};

# ![](dotnetimages/collapse.gif)Example

[Update File Raw References (C#)](Update_File_Raw_References_Example_CSharp.htm)

[Update File Raw References (VB.NET)](Update_File_Raw_References_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This structure is used by the [IEdmRawReferenceMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) interface.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRawReference Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional