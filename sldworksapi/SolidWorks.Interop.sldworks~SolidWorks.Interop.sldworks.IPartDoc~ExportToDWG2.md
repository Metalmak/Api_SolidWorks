<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ExportToDWG2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExportToDWG2 Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : ExportToDWG2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePath*
:   Path and file name of the exported DXF/DWG file

*ModelName*
:   Path and file name of the active part document

*Action*
:   Export action as defined in swExportToDWG\_e

*ExportToSingleFile*
:   True to save as one file; false to save as multiple files

*Alignment*
:   Array of 12 double values that contain information related to output alignment

*IsXDirFlipped*
:   True to flip the x direction; false otherwise

*IsYDirFlipped*
:   True to flip the y direction; false otherwise

*SheetMetalOptions*
:   Bitmask that contains sheet metal export options; valid only if Action = swExportToDWG\_e.swExportToDWG\_ExportSheetMetal

*Views*
:   Array of annotation view names to export; valid only if Action = swExportToDWG\_e.swExportToDWG\_ExportAnnotationViews

Saves various aspects of a part (sheet metal, faces, loops, and annotation views) to one or more DXF/DWG files, preserving the specified file name.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportToDWG2( _    ByVal FilePath As System.String, _    ByVal ModelName As System.String, _    ByVal Action As System.Integer, _    ByVal ExportToSingleFile As System.Boolean, _    ByVal Alignment As System.Object, _    ByVal IsXDirFlipped As System.Boolean, _    ByVal IsYDirFlipped As System.Boolean, _    ByVal SheetMetalOptions As System.Integer, _    ByVal Views As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim FilePath As System.String Dim ModelName As System.String Dim Action As System.Integer Dim ExportToSingleFile As System.Boolean Dim Alignment As System.Object Dim IsXDirFlipped As System.Boolean Dim IsYDirFlipped As System.Boolean Dim SheetMetalOptions As System.Integer Dim Views As System.Object Dim value As System.Boolean   value = instance.ExportToDWG2(FilePath, ModelName, Action, ExportToSingleFile, Alignment, IsXDirFlipped, IsYDirFlipped, SheetMetalOptions, Views) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ExportToDWG2(     System.string FilePath,    System.string ModelName,    System.int Action,    System.bool ExportToSingleFile,    System.object Alignment,    System.bool IsXDirFlipped,    System.bool IsYDirFlipped,    System.int SheetMetalOptions,    System.object Views ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ExportToDWG2(  &   System.String^ FilePath, &   System.String^ ModelName, &   System.int Action, &   System.bool ExportToSingleFile, &   System.Object^ Alignment, &   System.bool IsXDirFlipped, &   System.bool IsYDirFlipped, &   System.int SheetMetalOptions, &   System.Object^ Views ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePath*
:   Path and file name of the exported DXF/DWG file

*ModelName*
:   Path and file name of the active part document

*Action*
:   Export action as defined in swExportToDWG\_e

*ExportToSingleFile*
:   True to save as one file; false to save as multiple files

*Alignment*
:   Array of 12 double values that contain information related to output alignment

*IsXDirFlipped*
:   True to flip the x direction; false otherwise

*IsYDirFlipped*
:   True to flip the y direction; false otherwise

*SheetMetalOptions*
:   Bitmask that contains sheet metal export options; valid only if Action = swExportToDWG\_e.swExportToDWG\_ExportSheetMetal

*Views*
:   Array of annotation view names to export; valid only if Action = swExportToDWG\_e.swExportToDWG\_ExportAnnotationViews

#### Return Value

True if export is successful; false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::ExportToDWG2.

# ![](dotnetimages/collapse.gif)Example

[Export Part to DWG (VBA)](Export_Part_To_DWG_Example_VB.htm)

[Export Part to DWG (VB.NET)](Export_Part_To_DWG_Example_VBNET.htm)

[Export Part to DWG (C#)](Export_Part_To_DWG_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes IPartDoc::IExportToDWG by:

* Adding an option to SheetMetalOptions to export a sheet metal bounding box.* Not pre-pending the flat-pattern name to the FilePath file name of the exported DXF/DWG when ExportToSingleFile is false.

Alignment array is as follows:

> Array[0], Array[1], Array[2] - x,y,z coordinates of new origin
>
> Array[3], Array[4], Array[5] - coordinates of new x direction vector
>
> Array[6], Array[7], Array[8] - coordinates of new y direction vector
>
> Array[9], Array[10], Array[11] - coordinates of the vector that is normal to the selected faces or loops

The last three elements of the array are valid only if Action =swExportToDWG\_e.swExportToDWG\_ExportSelectedFacesOrLoops

The bitmask for SheetMetalOptions is {12 11 10 9 8 7 6 5 4 3 2 1}, where each bit is either 0 or 1 as follows:

> Bit #1: 1 to export flat-pattern geometry; 0 to not
>
> Bit #2: 1 to include hidden edges; 0 to not
>
> Bit #3: 1 to export bend lines; 0 to not
>
> Bit #4: 1 to include sketches; 0 to not
>
> Bit #5: 1 to merge coplanar faces; 0 to not
>
> Bit #6: 1 to export library features; 0 to not
>
> Bit #7: 1 to export forming tools; 0 to not
>
> Bit #8: 0
>
> Bit #9: 0
>
> Bit #10: 0
>
> Bit #11: 0
>
> Bit #12: 1 to export bounding box; 0 to not

For example, if you want to export:

* flat-pattern geometry, bend lines, and sketches, then Bits 1, 3, and 4 are 1, the bitmask is 0001101, and you need to set SheetMetalOptions = 2^0 + 2^2 + 2^3 = 1 + 4 + 8 = 13.

  * only the bounding box, then Bit 12 is 1, the bitmask is 100000000000, and you need to set SheetMetalOptions = 2^11 = 2048.

You must select multi-body sheet-metal features (i.e., multiple flat-pattern features) before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::IExportToDWG2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~IExportToDWG2.html)

[IPartDoc::ExportFlatPatternView Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ExportFlatPatternView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0