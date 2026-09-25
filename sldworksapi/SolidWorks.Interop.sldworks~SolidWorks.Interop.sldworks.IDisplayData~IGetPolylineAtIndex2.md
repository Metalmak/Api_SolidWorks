<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData~IGetPolylineAtIndex2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetPolylineAtIndex2 Method (IDisplayData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData.html) : IGetPolylineAtIndex2 Method (IDisplayData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of the desired polyline where the index begins at zero

Gets information for the specified polyline.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetPolylineAtIndex2( _    ByVal Index As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayData Dim Index As System.Integer Dim value As System.Double   value = instance.IGetPolylineAtIndex2(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetPolylineAtIndex2(     System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetPolylineAtIndex2(  &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of the desired polyline where the index begins at zero

#### Return Value

* in-process, unmanaged C++: Pointer to an array of doubles (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Format of return values is an array of doubles with the format:

> [ polyLineType, DataSize, Color, LineFont, Unused, Unused, NumPolyPoints, [x,y,z] ]

where:

|  |  |
| --- | --- |
| polyLineType | Underlying geometry type:  * 0 - Polyline type * 1 - Arc or Circle type |
| DataSize | Number of elements in the GeomData array. For Type = 0, this argument is 0. |
| Color | Polyline color. |
| LineFont | Polyline font information. You can use his value with [IDrawingDoc::GetLineFontInfo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~GetLineFontInfo2.html) and [IDrawingDoc::GetLineFontName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~GetLineFontName2.html). This value is valid only if LineStyle is -1. |
| NumPolyPoints | Number of XYZ points found in the [x,y,z] return value. |
| [x,y,z] | Array of points used to describe the polyline. This array has NumPolyPoints points. This method returns an array for every polyline regardless of its type. |

Use [IDisplayData::GetPolyLineSizeAtIndex2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayData~GetPolylineSizeAtIndex2.html) to determine the number of elements returned in this array.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData.html)

[IDisplayData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData_members.html)

[IDisplayData::GetPolylineAtIndex2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData~GetPolylineAtIndex2.html)

[IDisplayData::GetPolyLineCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData~GetPolyLineCount.html)

[IDisplayData::GetPolygonSizeAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayData~GetPolygonSizeAtIndex.html)