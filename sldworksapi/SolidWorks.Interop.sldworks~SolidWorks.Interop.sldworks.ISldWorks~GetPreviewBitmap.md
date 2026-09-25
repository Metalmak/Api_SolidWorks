<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmap.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPreviewBitmap Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetPreviewBitmap Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePathName*
:   Path and file name of the SOLIDWORKS document

*ConfigName*
:   Name of the configuration

Gets the preview bitmap (.bmp) for the specified configuration, regardless if the SOLIDWORKS document is open or closed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPreviewBitmap( _    ByVal FilePathName As System.String, _    ByVal ConfigName As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FilePathName As System.String Dim ConfigName As System.String Dim value As System.Object   value = instance.GetPreviewBitmap(FilePathName, ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPreviewBitmap(     System.string FilePathName,    System.string ConfigName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPreviewBitmap(  &   System.String^ FilePathName, &   System.String^ ConfigName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePathName*
:   Path and file name of the SOLIDWORKS document

*ConfigName*
:   Name of the configuration

#### Return Value

Dispatch pointer to IPictureDisp interface, the preview bitmap (.bmp) (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetPreviewBitmap.

# ![](dotnetimages/collapse.gif)Example

[Get Preview Bitmap (VBA)](Get_Preview_Bitmap_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The preview bitmap is the bitmap (.bmp) that appears in the Preview box on the Open dialog.

NOTES:

* Currently only in-process applications (that is, macros or add-ins) can use this method; out-of-process applications (that is, executables) will get an automation error because the IPictureDisp interface cannot be marshalled across process boundaries. This is a Microsoft behavior by design. See the Microsoft Knowledge Base for details.

  * This method is not supported in macros or out-of-process applications in SOLIDWORKS x64.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::PreviewDoc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreviewDoc.html)

[ISldWorks::PreviewDocx64 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreviewDocx64.html)

[ISldWorks::GetPreviewBitmapFile Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmapFile.html)

[IModelDoc2::SaveBMP Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SaveBMP.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 SP1, Revision Number 11.1