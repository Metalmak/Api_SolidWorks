<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureFillet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureFillet Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureFillet Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*
:   Feature fillet options as defined in swFeatureFilletOptions\_e

*R1*
:   Radius; valid only if:

    * Ftyp is not swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius* Options is set with swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e (see **Remarks**)

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

*Radii*
:   Array containing the radii for the variable radius fillet; valid only if:

    * Ftyp is set to swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options is set with swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options is not set with swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*SetBackDistances*
:   Array containing setback distances for the fillet along the edge

*PointRadiusArray*
:   Array containing control point radii at various points along the length of the edge; valid only if Ftyp is set to swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

Obsolete. Superseded by [IFeatureManager::FeatureFillet2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureFillet2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureFillet( _    ByVal Options As System.Integer, _    ByVal R1 As System.Double, _    ByVal Ftyp As System.Integer, _    ByVal OverflowType As System.Integer, _    ByVal Radii As System.Object, _    ByVal SetBackDistances As System.Object, _    ByVal PointRadiusArray As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Options As System.Integer Dim R1 As System.Double Dim Ftyp As System.Integer Dim OverflowType As System.Integer Dim Radii As System.Object Dim SetBackDistances As System.Object Dim PointRadiusArray As System.Object Dim value As System.Object   value = instance.FeatureFillet(Options, R1, Ftyp, OverflowType, Radii, SetBackDistances, PointRadiusArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.object FeatureFillet(     System.int Options,    System.double R1,    System.int Ftyp,    System.int OverflowType,    System.object Radii,    System.object SetBackDistances,    System.object PointRadiusArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ FeatureFillet(  &   System.int Options, &   System.double R1, &   System.int Ftyp, &   System.int OverflowType, &   System.Object^ Radii, &   System.Object^ SetBackDistances, &   System.Object^ PointRadiusArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   Feature fillet options as defined in swFeatureFilletOptions\_e

*R1*
:   Radius; valid only if:

    * Ftyp is not swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius* Options is set with swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e (see **Remarks**)

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

*Radii*
:   Array containing the radii for the variable radius fillet; valid only if:

    * Ftyp is set to swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options is set with swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options is not set with swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*SetBackDistances*
:   Array containing setback distances for the fillet along the edge

*PointRadiusArray*
:   Array containing control point radii at various points along the length of the edge; valid only if Ftyp is set to swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureFillet.

# ![](dotnetimages/collapse.gif)Remarks

| Before calling this method to create... | Do this... |
| --- | --- |
| Simple fillets | 1. Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 1 to select the edges to fillet.- Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_Simple. |
| Face blend fillets | 1. Call IModelDocExtension::SelectByID2 with:  + Mark = 2 to select the first set of faces.+ Mark = 4 to select the second set of faces.  2. Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_Face. |
| Variable radius fillets | 1. Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 1 to select the edges to fillet.- Call IModelDocExtension::SelectByID2 with Mark = 256 to select the control point references along the length of the selected edge, one control point reference for each radius in PointRadiusArray.- Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius.- Specify multiple radii in Radii.- Specify multiple control point radii in PointRadiusArray.- Do not set the Options parameter to swFeatureFilletOptions\_e.swFilletUniformRadius. |
| Full-round fillets | 1. Call IModelDocExtension::SelectByID2 with:  + Mark = 2 to select the first set of side faces.+ Mark = 512 to select the set of center faces.+ Mark = 4 to select the second set of side faces.  2. Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_FullRound. |
| Setback fillets | See the SOLIDWORKS Help for details. |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::FilletXpertChange Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertChange.html)

[IFeatureManager::FilletXpertRemove Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertRemove.html)

[IVariableFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html)

[ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[IFeatureManager::IFeatureFillet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IFeatureFillet.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0