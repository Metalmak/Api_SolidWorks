<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5~SaveBmp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SaveBmp Method (IEdmBitmap5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html) : SaveBmp Method (IEdmBitmap5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsBmpPath*
:   Path and name of the BMP file; if the file already exists, it is overwritten

Saves this bitmap image as a BMP file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SaveBmp( _    ByVal bsBmpPath As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SaveBmp(     System.string bsBmpPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SaveBmp(  &   System.String^ bsBmpPath ) ``` | |

#### Parameters

*bsBmpPath*
:   Path and name of the BMP file; if the file already exists, it is overwritten

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_SHARE\_ERROR: Error opening the file.* E\_EDM\_IO\_ERROR: Error writing the file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html)

[IEdmBitmap5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2