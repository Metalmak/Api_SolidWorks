<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar.html -->

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

| EdmRefVar Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRefVar Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Holds information about a single file reference variable; i.e., a variable stored on the reference relationship between an assembly file and one of its part files.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmRefVar     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmRefVar : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmRefVar : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmRefVar{
  integer [mlVarID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mlVarID.html);
  integer [mlParentFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mlParentFileID.html);
  integer [mlParentVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mlParentVersion.html);
  integer [mlChildFileID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mlChildFileID.html);
  string [mbsChildCfgName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mbsChildCfgName.html);
  string [mbsParentCfgName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mbsParentCfgName.html);
  object [moValue](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~moValue.html);
  integer [mhResult](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar~mhResult.html);
};

# ![](dotnetimages/collapse.gif)Example

[Batch Get and Set Reference Variables (VB.NET)](Batch_Get_and_Set_Reference_Variables_Example_VBNET.htm)

[Batch Get and Set Reference Variables (C#)](Batch_Get_and_Set_Reference_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Reference variables are used in Bill of Materials columns that are configured to look for reference-specific values. To create a reference variable:

1. Open the SOLIDWORKS PDM Professional Administration tool.- Log into a vault.- Double-click **Bill of Materials > BOM**.- Click a column in the **Columns** list.- Select **Look for variable in reference specific values**.- Click **OK**.- In a vault view, check out an assembly.- Click the **Bill of Materials** tab.- In the column configured to use reference-specific values, type text.- Click **Save** in the Bill of Materials toolbar.

Each component of the assembly is in a separate reference relationship with the assembly. The BOM column configured to **Look for variable in reference specific values** contains reference variable values. Use [IEdmBatchRefVars](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) to get and set these reference variable values.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmRefVar Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010