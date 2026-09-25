<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertChange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FilletXpertChange Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FilletXpertChange Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*
:   Feature fillet option as defined in swFeatureFilletOptions\_e

*R1*
:   Radius for uniform radius edge fillet

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

Changes the parameters on the selected filleted faces, regardless of whether the filleted faces were created manually or with FilletXpert, provided that FilletXpert can process them.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FilletXpertChange( _    ByVal Options As System.Integer, _    ByVal R1 As System.Double, _    ByVal Ftyp As System.Integer, _    ByVal OverflowType As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Options As System.Integer Dim R1 As System.Double Dim Ftyp As System.Integer Dim OverflowType As System.Integer Dim value As Feature   value = instance.FilletXpertChange(Options, R1, Ftyp, OverflowType) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FilletXpertChange(     System.int Options,    System.double R1,    System.int Ftyp,    System.int OverflowType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FilletXpertChange(  &   System.int Options, &   System.double R1, &   System.int Ftyp, &   System.int OverflowType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   Feature fillet option as defined in swFeatureFilletOptions\_e

*R1*
:   Radius for uniform radius edge fillet

*Ftyp*
:   Type of fillet as defined in swFeatureFilletType\_e

*OverflowType*
:   Control of fillet overflowing onto adjacent surfaces as defined in swFilletOverFlowType\_e

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FilletXpertChange.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::FeatureFillet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureFillet.html)

[IFeatureManager::FilletXpertRemove Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FilletXpertRemove.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0