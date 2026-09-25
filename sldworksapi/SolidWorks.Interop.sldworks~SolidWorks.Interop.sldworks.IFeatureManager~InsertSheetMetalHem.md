<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalHem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalHem Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetalHem Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type as defined in swHemTypes\_e

*Position*
:   Position as defined in swHemPositionTypes\_e

*Reverse*
:   True reverses the direction, false does not

*DLength*
:   Hem length; valid only for open or closed hems

*DGap*
:   Gap distance; valid only for open hems

*DAngle*
:   Hem angle; valid only for tear-drop or rolled hems

*DRad*
:   Hem radius; valid only for tear-drop or rolled hems

*DMiterGap*
:   Hem miter gap

*PCBA*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

Obsolete. Superseded by [IFeatureManager::InsertSheetMetalHem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertSheetMetalHem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetalHem( _    ByVal Type As System.Integer, _    ByVal Position As System.Integer, _    ByVal Reverse As System.Boolean, _    ByVal DLength As System.Double, _    ByVal DGap As System.Double, _    ByVal DAngle As System.Double, _    ByVal DRad As System.Double, _    ByVal DMiterGap As System.Double, _    ByVal PCBA As CustomBendAllowance _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim Position As System.Integer Dim Reverse As System.Boolean Dim DLength As System.Double Dim DGap As System.Double Dim DAngle As System.Double Dim DRad As System.Double Dim DMiterGap As System.Double Dim PCBA As CustomBendAllowance Dim value As Feature   value = instance.InsertSheetMetalHem(Type, Position, Reverse, DLength, DGap, DAngle, DRad, DMiterGap, PCBA) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetalHem(     System.int Type,    System.int Position,    System.bool Reverse,    System.double DLength,    System.double DGap,    System.double DAngle,    System.double DRad,    System.double DMiterGap,    CustomBendAllowance PCBA ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetalHem(  &   System.int Type, &   System.int Position, &   System.bool Reverse, &   System.double DLength, &   System.double DGap, &   System.double DAngle, &   System.double DRad, &   System.double DMiterGap, &   CustomBendAllowance^ PCBA ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type as defined in swHemTypes\_e

*Position*
:   Position as defined in swHemPositionTypes\_e

*Reverse*
:   True reverses the direction, false does not

*DLength*
:   Hem length; valid only for open or closed hems

*DGap*
:   Gap distance; valid only for open hems

*DAngle*
:   Hem angle; valid only for tear-drop or rolled hems

*DRad*
:   Hem radius; valid only for tear-drop or rolled hems

*DMiterGap*
:   Hem miter gap

*PCBA*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetalHem.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IHemFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHemFeatureData.html)

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0