<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundWidthFeature~GetPlaneFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetPlaneFeatures Method (ISwDMDimXpertCompoundWidthFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDimXpertCompoundWidthFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundWidthFeature.html) : GetPlaneFeatures Method (ISwDMDimXpertCompoundWidthFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Plane1*
:   [ISwDMDimXpertPlaneFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertPlaneFeature.html)

*Plane2*
:   [ISwDMDimXpertPlaneFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertPlaneFeature.html)

Gets the DimXpert plane features for both sides of this DimXpert compound width.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlaneFeatures( _    ByRef Plane1 As SwDMDimXpertPlaneFeature, _    ByRef Plane2 As SwDMDimXpertPlaneFeature _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDimXpertCompoundWidthFeature Dim Plane1 As SwDMDimXpertPlaneFeature Dim Plane2 As SwDMDimXpertPlaneFeature Dim value As System.Boolean   value = instance.GetPlaneFeatures(Plane1, Plane2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetPlaneFeatures(     out SwDMDimXpertPlaneFeature Plane1,    out SwDMDimXpertPlaneFeature Plane2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetPlaneFeatures(  &   [Out] SwDMDimXpertPlaneFeature^ Plane1, &   [Out] SwDMDimXpertPlaneFeature^ Plane2 ) ``` | |

#### Parameters

*Plane1*
:   [ISwDMDimXpertPlaneFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertPlaneFeature.html)

*Plane2*
:   [ISwDMDimXpertPlaneFeature](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDimXpertPlaneFeature.html)

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDimXpertCompoundWidthFeature::GetPlaneFeatures.

# ![](dotnetimages/collapse.gif)Example

See the examples on the interface page.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDimXpertCompoundWidthFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundWidthFeature.html)

[ISwDMDimXpertCompoundWidthFeature Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundWidthFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0