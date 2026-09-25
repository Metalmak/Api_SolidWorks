<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertLoftRefSurface2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertLoftRefSurface2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertLoftRefSurface2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Closed*
:   True for closed loft, false for open loft; if True, then you must have at least three profiles selected, and if you are using guide curves, the guide curves must be closed

*KeepTangency*
:   If the section curves are tangent, then you have the option to specify whether the resulting surfaces are also be tangent; specify True to maintain the tangency as seen in the section curves, false otherwise; when generating tangent surfaces, SOLIDWORKS maintains planar and cylindrical surface shapes if the section curves exhibit these characteristics

*ForceNonRational*
:   True to force the resulting surface to be non-rational, false to not

*TessToleranceFactor*
:   Factor to control the number of intermediate sections used for loft with centerline; default value is 1.0; the greater the variable, the more intermediate sections created

*StartMatchingType*
:   Tangency type at the start profile (see **Remarks**)

*EndMatchingType*
:   Tangency type at the end profile (see Remarks)

Creates a loft surface from the selected profiles, centerline, and guide curves.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertLoftRefSurface2( _    ByVal Closed As System.Boolean, _    ByVal KeepTangency As System.Boolean, _    ByVal ForceNonRational As System.Boolean, _    ByVal TessToleranceFactor As System.Double, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Closed As System.Boolean Dim KeepTangency As System.Boolean Dim ForceNonRational As System.Boolean Dim TessToleranceFactor As System.Double Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short   instance.InsertLoftRefSurface2(Closed, KeepTangency, ForceNonRational, TessToleranceFactor, StartMatchingType, EndMatchingType) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertLoftRefSurface2(     System.bool Closed,    System.bool KeepTangency,    System.bool ForceNonRational,    System.double TessToleranceFactor,    System.short StartMatchingType,    System.short EndMatchingType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertLoftRefSurface2(  &   System.bool Closed, &   System.bool KeepTangency, &   System.bool ForceNonRational, &   System.double TessToleranceFactor, &   System.short StartMatchingType, &   System.short EndMatchingType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Closed*
:   True for closed loft, false for open loft; if True, then you must have at least three profiles selected, and if you are using guide curves, the guide curves must be closed

*KeepTangency*
:   If the section curves are tangent, then you have the option to specify whether the resulting surfaces are also be tangent; specify True to maintain the tangency as seen in the section curves, false otherwise; when generating tangent surfaces, SOLIDWORKS maintains planar and cylindrical surface shapes if the section curves exhibit these characteristics

*ForceNonRational*
:   True to force the resulting surface to be non-rational, false to not

*TessToleranceFactor*
:   Factor to control the number of intermediate sections used for loft with centerline; default value is 1.0; the greater the variable, the more intermediate sections created

*StartMatchingType*
:   Tangency type at the start profile (see **Remarks**)

*EndMatchingType*
:   Tangency type at the end profile (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertLoftRefSurface2.

# ![](dotnetimages/collapse.gif)Remarks

Selection of guide curves and centerline is optional; however, selection of the profiles must be in an order consistent with the desired direction of the loft. Because you are creating a surface, the section profiles can be open.

Use of guide curves is strongly recommended, especially when selection of profiles is done in the FeatureManager design tree.

You can use any number of profiles; however, if you have selected only one profile, then any selected guide curves must be closed curves.

Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select the profiles and guide curves. The mark for:

* profile selections should be 1

  * any guide curve selection, if provided, should be 2

    * centerline selection, if provided, should be 4

      * start tangency vector selection, if provided, should be an 8

        * start tangency faces selection, if provided, should be a 16 (not available currently

          * end tangency vector selection, if provided, should be a 32

            * end tangency faces selection, if provided, should be a 64 (not available currently)

Linear edge, sketch line, axis, plane and planar faces are qualified for tangency vector sections.

The tangency types can be one of the following:

|  |  |
| --- | --- |
| 0  = | none |
| 1  = | tangent to the normal of the profile |
| 2  = | tangent to a selected vector |
| 3  = | tangency to all the adjacent faces sharing an edge with the start profile |
| 4  = | tangent to some of the selected faces sharing an edge with the start profile (not available at this moment). |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IFeatureManager::InsertProtrusionBlend Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertProtrusionBlend.html)

[IFeatureManager::InsertCutBlend Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCutBlend.html)

[ILoftFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftFeatureData.html)

[IModeler::CreateLoftSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateLoftSurface.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0