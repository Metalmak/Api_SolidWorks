<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompositeDistanceBetweenDimTol~GetUpperAndLowerLimitIntraFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetUpperAndLowerLimitIntraFeature Method (IDimXpertCompositeDistanceBetweenDimTol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertCompositeDistanceBetweenDimTol Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompositeDistanceBetweenDimTol.html) : GetUpperAndLowerLimitIntraFeature Method (IDimXpertCompositeDistanceBetweenDimTol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Upper*
:   Upper limit

*Lower*
:   Lower limit

Gets the upper and lower tolerance limits for the feature-locating portion of this DimXpert composite distance-between dimension tolerance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetUpperAndLowerLimitIntraFeature( _    ByRef Upper As System.Double, _    ByRef Lower As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertCompositeDistanceBetweenDimTol Dim Upper As System.Double Dim Lower As System.Double Dim value As System.Boolean   value = instance.GetUpperAndLowerLimitIntraFeature(Upper, Lower) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetUpperAndLowerLimitIntraFeature(     out System.double Upper,    out System.double Lower ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetUpperAndLowerLimitIntraFeature(  &   [Out] System.double Upper, &   [Out] System.double Lower ) ``` | |

#### Parameters

*Upper*
:   Upper limit

*Lower*
:   Lower limit

#### Return Value

True if the method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertCompositeDistanceBetweenDimTol::GetUpperAndLowerLimitIntraFeature.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertCompositeDistanceBetweenDimTol Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompositeDistanceBetweenDimTol.html)

[IDimXpertCompositeDistanceBetweenDimTol Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompositeDistanceBetweenDimTol_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0