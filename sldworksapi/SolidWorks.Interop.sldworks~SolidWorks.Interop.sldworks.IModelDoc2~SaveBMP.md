<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SaveBMP.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveBMP Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SaveBMP Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileNameIn*
:   Path and file name of the new BMP file

*WidthIn*
:   Width of the BMP

*HeightIn*
:   Height of the BMP

Saves the current view as a bitmap (BMP) file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveBMP( _    ByVal FileNameIn As System.String, _    ByVal WidthIn As System.Integer, _    ByVal HeightIn As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim FileNameIn As System.String Dim WidthIn As System.Integer Dim HeightIn As System.Integer Dim value As System.Boolean   value = instance.SaveBMP(FileNameIn, WidthIn, HeightIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveBMP(     System.string FileNameIn,    System.int WidthIn,    System.int HeightIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveBMP(  &   System.String^ FileNameIn, &   System.int WidthIn, &   System.int HeightIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileNameIn*
:   Path and file name of the new BMP file

*WidthIn*
:   Width of the BMP

*HeightIn*
:   Height of the BMP

#### Return Value

True if file is created successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SaveBMP.

# ![](dotnetimages/collapse.gif)Example

[Save Model as Bitmap (C#)](Save_Model_as_Bitmap_Example_CSharp.htm)

[Save Model as Bitmap (VB.NET)](Save_Model_as_Bitmap_Example_VBNET.htm)

[Save Model as Bitmap (VBA)](Save_Model_as_Bitmap_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Include the full path to the file in FilenameIn and use filename extension of .bmp.

If WidthIn or the HeightIn is less than or equal to 0, then the view size is based on the current window size.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[ISldWorks::GetPreviewBitmapFile Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmapFile.html)

[ISldWorks::GetPreviewBitmap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetPreviewBitmap.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0