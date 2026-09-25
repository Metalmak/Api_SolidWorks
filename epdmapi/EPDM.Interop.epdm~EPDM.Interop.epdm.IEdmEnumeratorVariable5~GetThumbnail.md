<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetThumbnail.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetThumbnail Method (IEdmEnumeratorVariable5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) : GetThumbnail Method (IEdmEnumeratorVariable5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets a preview bitmap of the current file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetThumbnail() As IEdmBitmap5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmBitmap5 GetThumbnail() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmBitmap5^ GetThumbnail(); ``` | |

#### Return Value

[IEdmBitmap5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html); Null if the file does not support bitmap previews

# ![](dotnetimages/collapse.gif)Example

[Get Preview Bitmap of File (VB.NET)](Get_Bitmap_Preview_of_File_Example_VBNET.htm)

[Get Preview Bitmap of File (C#)](Get_Bitmap_Preview_of_File_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supports only DWG files that are cached.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmBitmap5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The file does not support bitmap previews.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html)

[IEdmEnumeratorVariable5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2