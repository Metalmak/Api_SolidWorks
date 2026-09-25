<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureLocalSketchDrivenPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureLocalSketchDrivenPattern Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureLocalSketchDrivenPattern Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReferencePoint*
:   Type of selected reference point as defined in swLocalSketchPatternReferencePoint\_e (see **Remarks**)

Obsolete. See [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and the Remarks in [ILocalSketchPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalSketchPatternFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureLocalSketchDrivenPattern( _    ByVal ReferencePoint As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim ReferencePoint As System.Integer Dim value As Feature   value = instance.FeatureLocalSketchDrivenPattern(ReferencePoint) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureLocalSketchDrivenPattern(     System.int ReferencePoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureLocalSketchDrivenPattern(  &   System.int ReferencePoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReferencePoint*
:   Type of selected reference point as defined in swLocalSketchPatternReferencePoint\_e (see **Remarks**)

#### Return Value

Local sketch pattern [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureLocalSketchDrivenPattern.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **To** [**select**](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html)**...** | **Use a mark of...** |
| Components to pattern | 1 |
| Sketch to define the pattern | 16 |
| Reference point for ReferencePoint  **NOTE:** If ReferencePoint is set to swLocalSketchPatternReferencePoint\_e.swLocalSketchPatternSelectedPoint, then the selected reference point must be a vertex. | 32 |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0