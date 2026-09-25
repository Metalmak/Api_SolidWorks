<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextParent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextParent Method (IEdmReference5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) : GetNextParent Method (IEdmReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of the next parent file to get

Enumerates the files referencing this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextParent( _    ByVal poPos As IEdmPos5 _ ) As IEdmReference5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmReference5 GetNextParent(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmReference5^ GetNextParent(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [Position](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) of the next parent file to get

#### Return Value

Parent [file](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

# ![](dotnetimages/collapse.gif)Example

[Get Parent References of File (VB.NET)](Get_Parent_References_Example_VBNET.htm)

[Get Parent References of File (C#)](Get_Parent_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [IEdmReference7::GetFirstParentPosition2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstParentPosition2.html) to get the position of the first referenced parent file, before you call this method the first time.

After calling this method the first time, poPos is automatically incremented every time this method is called. Call this method repeatedly to obtain the rest of the referenced parent files.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional