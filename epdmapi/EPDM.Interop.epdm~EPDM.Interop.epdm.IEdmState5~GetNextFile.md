<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetNextFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextFile Method (IEdmState5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : GetNextFile Method (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPosition*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next file in this workflow state (see **Remarks**)

Gets the next file in this workflow state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextFile( _    ByVal poPosition As IEdmPos5 _ ) As IEdmFile5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFile5 GetNextFile(     IEdmPos5 poPosition ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFile5^ GetNextFile(  &   IEdmPos5^ poPosition ) ``` | |

#### Parameters

*poPosition*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next file in this workflow state (see **Remarks**)

#### Return Value

[IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

# ![](dotnetimages/collapse.gif)Example

[Get Files in Workflow State (VB.NET)](Get_Files_in_State_Example_VBNET.htm)

[Get Files in Workflow State (C#)](Get_Files_in_State_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPosition with the interface to the position of the first file, IEdmPos5. Call [IEdmState5::GetFirstFilePosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetFirstFilePosition.html) to start an enumeration and obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the files.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers must free the interface returned, IEdmFile5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2