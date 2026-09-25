<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html -->

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

| EdmAddInFileInfo Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddInFileInfo Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a single file in an add-in package.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmAddInFileInfo     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmAddInFileInfo : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmAddInFileInfo : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmAddInFileInfo{
  string  [mbsFileName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo~mbsFileName.html);
  integer [mlEdmAddInFileInfoFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo~mlEdmAddInFileInfoFlags.html);
};

# ![](dotnetimages/collapse.gif)Example

[Install Add-in (VB.NET)](Load_Addin_Example_VBNET.htm)

[Install Add-in (C#)](Load_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Returned by [IEdmAddInMgr8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EdmAddInFileInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010