<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5~GetBitmapInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetBitmapInfo Method (IEdmBitmap5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html) : GetBitmapInfo Method (IEdmBitmap5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDataSize*
:   Size of pbData (see **Remarks**)

*pbData*
:   Buffer in which to return the bitmap information

Gets bitmap information.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetBitmapInfo( _    ByVal lDataSize As System.Integer, _    ByRef pbData As System.Byte _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetBitmapInfo(     System.int lDataSize,    out System.byte pbData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetBitmapInfo(  &   System.int lDataSize, &   [Out] System.byte pbData ) ``` | |

#### Parameters

*lDataSize*
:   Size of pbData (see **Remarks**)

*pbData*
:   Buffer in which to return the bitmap information

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must properly allocate the size of the pbData buffer. Call [IEdmBitmap5::GetBitmapInfoSize](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5~GetBitmapInfoSize.html) to determine the size of buffer to allocate and to specify lDataSize.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_INVALIDARG: lDataSize does not match the size of the returned structure.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html)

[IEdmBitmap5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2