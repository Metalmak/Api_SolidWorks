<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument~SaveCompareVolumeResults.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SaveCompareVolumeResults Method (ICompareDocument) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [ICompareDocument Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument.html) : SaveCompareVolumeResults Method (ICompareDocument) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*resultfile*
:   Path and filename to which to save the SOLIDWORKS part document

    NOTE: You do not have to specify the filename extension .sldprt. It is automatically appended to the filename.

Saves the volume comparison results as a SOLIDWORKS part document after comparing documents with the Compare volumes option selected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveCompareVolumeResults( _    ByVal resultfile As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompareDocument Dim resultfile As System.String Dim value As System.Integer   value = instance.SaveCompareVolumeResults(resultfile) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SaveCompareVolumeResults(     System.string resultfile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SaveCompareVolumeResults(  &   System.String^ resultfile ) ``` | |

#### Parameters

*resultfile*
:   Path and filename to which to save the SOLIDWORKS part document

    NOTE: You do not have to specify the filename extension .sldprt. It is automatically appended to the filename.

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ICompareDocument::SaveCompareVolumeResults.

# ![](dotnetimages/collapse.gif)See Also

####

[ICompareDocument Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument.html)

[ICompareDocument Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS