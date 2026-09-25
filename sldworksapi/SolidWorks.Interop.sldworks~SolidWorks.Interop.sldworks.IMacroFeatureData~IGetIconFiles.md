<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetIconFiles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetIconFiles Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : IGetIconFiles Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IconCount*
:   Number of files for the icons

*IconFiles*
:   * in-process, unmanaged C++: Pointer to an array of file names for the icons (see **Remarks)**

    * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Gets the file names for the icons for this macro feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetIconFiles( _    ByVal IconCount As System.Integer, _    ByRef IconFiles As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim IconCount As System.Integer Dim IconFiles As System.String   instance.IGetIconFiles(IconCount, IconFiles) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetIconFiles(     System.int IconCount,    out System.string IconFiles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetIconFiles(  &   System.int IconCount, &   [Out] System.String^ IconFiles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IconCount*
:   Number of files for the icons

*IconFiles*
:   * in-process, unmanaged C++: Pointer to an array of file names for the icons (see **Remarks)**

    * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IMacroFeatureData::GetIconFileCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~GetIconFileCount.html) to determine the size of the array.

The array of the file names for IconFiles can contain either three or nine strings.

| Number of strings in array | Types of images in this order | Image format and sizes |
| --- | --- | --- |
| Three | 1. Regular- Suppressed- Highlighted | * Windows bitmap (**\*.bmp**) format* 16 pixels wide X 18 pixels high |
| Nine  **NOTES:**   * This size array is only valid for macro features created in parts, assemblies, and drawings in SOLIDWORKS 2017 and later.* SOLIDWORKS displays the appropriate images based on the current DPI setting of the display device. | 1. Regular small- Suppressed small- Highlighted small- Regular medium- Suppressed medium- Highlighted medium- Regular large- Suppressed large- Highlighted large | * Windows bitmap (**\*.bmp**) format* Recommended sizes are:     + Small: 20 pixels wide X 20 pixels high+ Medium: 32 pixels wide X 32 pixels high+ Large: 40 pixels wide X 40 pixels high |

You can specify either the full path name or just the file name for the strings; for example, c:\bitmaps\icon1.bmp or icon1.bmp.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

[IMacroFeatureData::ISetIconFiles Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetIconFiles.html)

[IMacroFeatureData::IconFiles Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IconFiles.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0