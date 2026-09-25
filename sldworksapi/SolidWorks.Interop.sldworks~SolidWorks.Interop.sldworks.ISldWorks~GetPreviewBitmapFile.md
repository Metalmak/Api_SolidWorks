<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmapFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPreviewBitmapFile Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetPreviewBitmapFile Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocumentPath*
:   Path and file name of the SOLIDWORKS document whose preview bitmap (.bmp) you want to save

*ConfigName*
:   Name of the configuration

*BitMapFile*
:   Filename for the preview

Gets the specified preview bitmap of a document and saves it as a Windows bitmap file (.bmp) using the specified filename.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPreviewBitmapFile( _    ByVal DocumentPath As System.String, _    ByVal ConfigName As System.String, _    ByVal BitMapFile As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocumentPath As System.String Dim ConfigName As System.String Dim BitMapFile As System.String Dim value As System.Boolean   value = instance.GetPreviewBitmapFile(DocumentPath, ConfigName, BitMapFile) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetPreviewBitmapFile(     System.string DocumentPath,    System.string ConfigName,    System.string BitMapFile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetPreviewBitmapFile(  &   System.String^ DocumentPath, &   System.String^ ConfigName, &   System.String^ BitMapFile ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocumentPath*
:   Path and file name of the SOLIDWORKS document whose preview bitmap (.bmp) you want to save

*ConfigName*
:   Name of the configuration

*BitMapFile*
:   Filename for the preview

#### Return Value

True if the preview bitmap (.bmp) is saved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetPreviewBitmapFile.

# ![](dotnetimages/collapse.gif)Example

[Save Configuration Data (C#)](Save_Configuration_Data_Example_CSharp.htm)

[Save Configuration Data (VB.NET)](Save_Configuration_Data_Example_VBNET.htm)

[Save Configuration Data (VBA)](Save_Configuration_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetPreviewBitmap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmap.html)

[ISldWorks::PreviewDoc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreviewDoc.html)

[ISldWorks::PreviewDocx64 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~PreviewDocx64.html)

[IModelDoc2::SaveBMP Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SaveBMP.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 Sp2, Revision Number 16.2