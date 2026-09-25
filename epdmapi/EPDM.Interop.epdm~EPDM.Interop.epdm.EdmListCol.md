<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol.html -->

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

| EdmListCol Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmListCol Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a column in a file listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmListCol     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmListCol : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmListCol : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmListCol{
  string [mbsCaption](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~mbsCaption.html);
  integer [mlEdmListColFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~mlEdmListColFlags.html);
  enum [EdmColType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmColType.html) [meColType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~meColType.html);
  integer [mlVariableID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~mlVariableID.html);
  enum [EdmVariableType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableType.html) [meVarType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~meVarType.html);
  integer [mlWidth](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol~mlWidth.html);
}

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Also see the [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) examples.

This structure is returned by [IEdmSearchResult6::GetCustomColumnsInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnsInfo.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListCol Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListCol_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional