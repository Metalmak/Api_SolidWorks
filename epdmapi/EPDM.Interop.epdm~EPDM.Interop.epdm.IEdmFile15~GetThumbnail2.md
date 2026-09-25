<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile15~GetThumbnail2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetThumbnail2 Method (IEdmFile15) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile15 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile15.html) : GetThumbnail2 Method (IEdmFile15) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersion*
:   Version of the file whose thumbnail to retrieve

Gets this file's thumbnail by file version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetThumbnail2( _    ByVal lVersion As System.Integer _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetThumbnail2(     System.int lVersion ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetThumbnail2(  &   System.int lVersion ) ``` | |

#### Parameters

*lVersion*
:   Version of the file whose thumbnail to retrieve

#### Return Value

IPicture

# ![](dotnetimages/collapse.gif)Example

[Get a File's Thumbnail by File Version (C#)](Get_File_Thumbnail_by_Version_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If a thumbnail of this file is not available, this method returns Nothing or null.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile15 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile15.html)

[IEdmFile15 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile15_members.html)

[IEdmEnumeratorVariable5::GetThumbnail Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetThumbnail.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018 SP04