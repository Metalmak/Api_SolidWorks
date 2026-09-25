<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextChild.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextChild Method (IEdmReference5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) : GetNextChild Method (IEdmReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of next child file to get

Enumerates the files referenced by this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextChild( _    ByVal poPos As IEdmPos5 _ ) As IEdmReference5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmReference5 GetNextChild(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmReference5^ GetNextChild(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of next child file to get

#### Return Value

Child [file](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [IEdmReference5::GetFirstChildPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetFirstChildPosition.html) to get the position of the first referenced child file, before you call IEdmReference5::GetNextChild for the first time.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the referenced child files.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional