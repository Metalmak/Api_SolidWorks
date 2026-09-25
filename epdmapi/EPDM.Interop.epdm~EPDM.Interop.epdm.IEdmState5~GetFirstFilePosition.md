<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetFirstFilePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstFilePosition Method (IEdmState5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : GetFirstFilePosition Method (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of all the files in this workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstFilePosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstFilePosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstFilePosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position in the list of the first file in this workflow state (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Get Files in Workflow State (VB.NET)](Get_Files_in_State_Example_VBNET.htm)

[Get Files in Workflow State (C#)](Get_Files_in_State_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first file in this workflow state to [IEdmState5::GetNextFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetNextFile.html) to get the first file in this workflow state. Then call IEdmState5::GetNextFile repeatedly to get the rest of the files in this workflow state.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

Use [IEdmSearch5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) to perform more elaborate searches.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2