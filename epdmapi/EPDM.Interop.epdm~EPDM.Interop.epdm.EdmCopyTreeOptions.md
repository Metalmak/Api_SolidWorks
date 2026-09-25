<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions.html -->

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

| EdmCopyTreeOptions Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmCopyTreeOptions Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains options for copying an assembly tree of files to a destination folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmCopyTreeOptions     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmCopyTreeOptions : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmCopyTreeOptions : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmCmdInfo

{
  string [mbsPrefix](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions~mbsPrefix.html);
  string [mbsSuffix](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions~mbsSuffix.html);
  VARIANT\_BOOL [mbIncludeDrawings](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions~mbIncludeDrawings.html);
  VARIANT\_BOOL [mbUseLatestVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions~mbUseLatestVersion.html);
};

# ![](dotnetimages/collapse.gif)Example

[Copy Assembly Tree of Files (VB.NET)](Copy_Assembly_Tree_Example_VBNET.htm)

[Copy Assembly Tree of Files (C#)](Copy_Assembly_Tree_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmCopyTreeOptions Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyTreeOptions_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)