<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureFillet2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureFillet2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureFillet2 Method (IFeatureManager) |

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
:   Uniform radius of the fillet; valid only if:

    * Ftyp != swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius* Options include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*Rho*
:   Value that determines the conic shape of the fillet:

    * Conic rho value [0.05, 0.95], if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletConicRho (see **Remarks**)* Conic radius value, if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletConicRadius* Circular radius value, if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletCircular

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e (see **Remarks**)

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

*ConicRhoType*
:   Conic fillet profile type as defined in swFeatureFilletProfileType\_e

*Radii*
:   Array containing the radii for the variable radius fillet; valid only if:

    * Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options include swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options do not include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*RhoArr*
:   Array of Rho values for the specified ConicRhoType for the variable radius fillet; valid only if:

    * Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options include swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options do not include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*SetBackDistances*
:   Array containing setback distances along the fillet edge

*PointRadiusArray*
:   Array containing radii at various control points along the length of the edge; valid only if Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

*PointRhoArray*
:   Array of Rho values for the specified ConicRhoType at various control points along the length of the edge; valid only if Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

Obsolete. Superseded by [IFeatureManager::FeatureFillet3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureFillet3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureFillet2( _    ByVal Options As System.Integer, _    ByVal R1 As System.Double, _    ByVal Rho As System.Double, _    ByVal Ftyp As System.Integer, _    ByVal OverflowType As System.Integer, _    ByVal ConicRhoType As System.Integer, _    ByVal Radii As System.Object, _    ByVal RhoArr As System.Object, _    ByVal SetBackDistances As System.Object, _    ByVal PointRadiusArray As System.Object, _    ByVal PointRhoArray As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Options As System.Integer Dim R1 As System.Double Dim Rho As System.Double Dim Ftyp As System.Integer Dim OverflowType As System.Integer Dim ConicRhoType As System.Integer Dim Radii As System.Object Dim RhoArr As System.Object Dim SetBackDistances As System.Object Dim PointRadiusArray As System.Object Dim PointRhoArray As System.Object Dim value As System.Object   value = instance.FeatureFillet2(Options, R1, Rho, Ftyp, OverflowType, ConicRhoType, Radii, RhoArr, SetBackDistances, PointRadiusArray, PointRhoArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.object FeatureFillet2(     System.int Options,    System.double R1,    System.double Rho,    System.int Ftyp,    System.int OverflowType,    System.int ConicRhoType,    System.object Radii,    System.object RhoArr,    System.object SetBackDistances,    System.object PointRadiusArray,    System.object PointRhoArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ FeatureFillet2(  &   System.int Options, &   System.double R1, &   System.double Rho, &   System.int Ftyp, &   System.int OverflowType, &   System.int ConicRhoType, &   System.Object^ Radii, &   System.Object^ RhoArr, &   System.Object^ SetBackDistances, &   System.Object^ PointRadiusArray, &   System.Object^ PointRhoArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   Feature fillet options as defined in swFeatureFilletOptions\_e

*R1*
:   Uniform radius of the fillet; valid only if:

    * Ftyp != swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius* Options include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*Rho*
:   Value that determines the conic shape of the fillet:

    * Conic rho value [0.05, 0.95], if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletConicRho (see **Remarks**)* Conic radius value, if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletConicRadius* Circular radius value, if ConicRhoType = swFeatureFilletProfileType\_e.swFeatureFilletCircular

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e (see **Remarks**)

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

*ConicRhoType*
:   Conic fillet profile type as defined in swFeatureFilletProfileType\_e

*Radii*
:   Array containing the radii for the variable radius fillet; valid only if:

    * Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options include swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options do not include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*RhoArr*
:   Array of Rho values for the specified ConicRhoType for the variable radius fillet; valid only if:

    * Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

      * Options include swFeatureFilletOptions\_e.swFeatureFilletVarRadiusType

        * Options do not include swFeatureFilletOptions\_e.swFeatureFilletUniformRadius

*SetBackDistances*
:   Array containing setback distances along the fillet edge

*PointRadiusArray*
:   Array containing radii at various control points along the length of the edge; valid only if Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

*PointRhoArray*
:   Array of Rho values for the specified ConicRhoType at various control points along the length of the edge; valid only if Ftyp = swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureFillet2.

# ![](dotnetimages/collapse.gif)Remarks

If the conic rho value specified in parameter, Rho, is not in the valid range, then this method replaces it with the closest value in the valid range. For example, 0.01 is replaced by 0.05, and 0.99 is replaced by 0.95.

| Before calling this method to create... | You must... |
| --- | --- |
| Simple fillets | 1. Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 1 to select the edges to fillet.- Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_Simple. |
| Face blend fillets | 1. Call IModelDocExtension::SelectByID2 with:  + Mark = 2 to select the first set of faces.+ Mark = 4 to select the second set of faces.  2. Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_Face. |
| Variable radius fillets | 1. Call IModelDocExtension::SelectByID2 with Mark = 1 to select the edges to fillet.- Call IModelDocExtension::SelectByID2 with Mark = 256 to select the control point references along the length of the selected edge; one control point reference for each radius in PointRadiusArray.- Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_VariableRadius.- Specify multiple radii in Radii.- Specify multiple control point radii in PointRadiusArray.- Do not include swFeatureFilletOptions\_e.swFilletUniformRadius in Options. |
| Full-round fillets | 1. Call IModelDocExtension::SelectByID2 with:  + Mark = 2 to select the first set of side faces.+ Mark = 512 to select the set of center faces.+ Mark = 4 to select the second set of side faces.  2. Specify Ftyp with swFeatureFilletType\_e.swFeatureFilletType\_FullRound. |
| Setback fillets | See the SOLIDWORKS Help for details. |
| Conic fillets | See the SOLIDWORKS Help for details. |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::IFeatureFillet2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IFeatureFillet2.html)

[ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[IVariableFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html)

[IFeatureManager::FilletXpertChange Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertChange.html)

[IFeatureManager::FilletXpertMakeCorner Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertMakeCorner.html)

[IFeatureManager::FilletXpertRemove Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertRemove.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0