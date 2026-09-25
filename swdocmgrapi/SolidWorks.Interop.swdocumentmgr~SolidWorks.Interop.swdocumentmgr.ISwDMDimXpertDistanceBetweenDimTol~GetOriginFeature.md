<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertDistanceBetweenDimTol~GetOriginFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetOriginFeature Method (ISwDMDimXpertDistanceBetweenDimTol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDimXpertDistanceBetweenDimTol Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertDistanceBetweenDimTol.html) : GetOriginFeature Method (ISwDMDimXpertDistanceBetweenDimTol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Feature*
:   [ISwDMDimXpertFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertFeature.html)

*FosUsage*
:   How to treat the feature of size when applying this tolerance as defined in [swDmDimXpertDistanceFosUsage\_e](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.swDmDimXpertDistanceFosUsage_e.html)

Gets the DimXpert feature of origin for this DimXpert distance-between dimension tolerance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetOriginFeature( _    ByRef Feature As SwDMDimXpertFeature, _    ByRef FosUsage As swDmDimXpertDistanceFosUsage_e _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDimXpertDistanceBetweenDimTol Dim Feature As SwDMDimXpertFeature Dim FosUsage As swDmDimXpertDistanceFosUsage_e Dim value As System.Boolean   value = instance.GetOriginFeature(Feature, FosUsage) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetOriginFeature(     out SwDMDimXpertFeature Feature,    out swDmDimXpertDistanceFosUsage_e FosUsage ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetOriginFeature(  &   [Out] SwDMDimXpertFeature^ Feature, &   [Out] swDmDimXpertDistanceFosUsage_e FosUsage ) ``` | |

#### Parameters

*Feature*
:   [ISwDMDimXpertFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertFeature.html)

*FosUsage*
:   How to treat the feature of size when applying this tolerance as defined in [swDmDimXpertDistanceFosUsage\_e](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.swDmDimXpertDistanceFosUsage_e.html)

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDimXpertDistanceBetweenDimTol::GetOriginFeature.

# ![](dotnetimages/collapse.gif)Example

See the examples on the interface page.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDimXpertDistanceBetweenDimTol Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertDistanceBetweenDimTol.html)

[ISwDMDimXpertDistanceBetweenDimTol Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertDistanceBetweenDimTol_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0