<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile13~GetThumbnail.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetThumbnail Method (IEdmFile13) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile13.html) : GetThumbnail Method (IEdmFile13) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [IEdmFile15::GetThumbnail2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile15~GetThumbnail2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetThumbnail() As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetThumbnail() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetThumbnail(); ``` | |

#### Return Value

IPicture

# ![](dotnetimages/collapse.gif)Example

'This code snippet demonstrates how to convert the IPicture object returned by this method to a usable bitmap.

VB.NET:

```
Imports stdole
Imports System
Imports System.Drawing
Imports System.Windows.Forms
```

```
Module Module1

    Sub Main()
```

```
       ...
```

```
       Dim objBitMap As Object = aFile.GetThumbnail
       Dim imgPreview As System.Drawing.Image = PictureDispConverter.Convert(objBitMap)
       imgPreview.Save(sExtractDir + sFilename + ".bmp", Drawing.Imaging.ImageFormat.Bmp)
       imgPreview.Dispose()

    End Sub

End Module

'Class1
Public Class PictureDispConverter

    Inherits System.Windows.Forms.AxHost

    Public Sub New()
        MyBase.New("GUID_format5_value")
    End Sub

    Public Shared Function Convert(ByVal objIDispImage As Object) As System.Drawing.Image
        Dim objPicture As System.Drawing.Image
        objPicture = CType(System.Windows.Forms.AxHost.GetPictureFromIPicture(objIDispImage), System.Drawing.Image)
        Return objPicture
    End Function

End Class
```

# ![](dotnetimages/collapse.gif)Remarks

If a thumbnail of this file is not available, this method returns Nothing or null.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile13 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile13.html)

[IEdmFile13 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile13_members.html)

[IEdmEnumeratorVariable5::GetThumbnail Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~GetThumbnail.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018