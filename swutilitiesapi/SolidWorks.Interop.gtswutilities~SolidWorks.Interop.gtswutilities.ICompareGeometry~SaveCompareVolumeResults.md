<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry~SaveCompareVolumeResults.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SaveCompareVolumeResults Method (ICompareGeometry) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [ICompareGeometry Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry.html) : SaveCompareVolumeResults Method (ICompareGeometry) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*resultfile*
:   Path and file name for the SOLIDWORKS part document (see **Remarks**)

    NOTE: You do not have to specify the filename extension .sldprt. It is automatically appended to the file name.

Obsolete. Do not use.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveCompareVolumeResults( _    ByVal resultfile As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompareGeometry Dim resultfile As System.String Dim value As System.Integer   value = instance.SaveCompareVolumeResults(resultfile) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SaveCompareVolumeResults(     System.string resultfile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SaveCompareVolumeResults(  &   System.String^ resultfile ) ``` | |

#### Parameters

*resultfile*
:   Path and file name for the SOLIDWORKS part document (see **Remarks**)

    NOTE: You do not have to specify the filename extension .sldprt. It is automatically appended to the file name.

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ICompareGeometry::SaveCompareVolumeResults.

# ![](dotnetimages/collapse.gif)Remarks

This method opens the volume comparison results in a SOLIDWORKS part document after comparing geometry with the **Perform volume comparison** option selected.

If only a directory is specified in resultfile, a part document named "Volume Comparison of <part 1> and <part 2>.sldprt" is opened (but not saved) in SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[ICompareGeometry Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry.html)

[ICompareGeometry Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS