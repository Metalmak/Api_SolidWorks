<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetal3dBend.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetal3dBend Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetal3dBend Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   Angle of the bend in radians

*BUseDefaultRadius*
:   True to use the default radius, false to use the value specified in radius

*Radius*
:   Value for the radius of the bend if bUseDefaultRadius is false

*FlipDir*
:   True to flip the bend direction, false to not

*BendPos*
:   Bend position:

    * 0 = bend centerline

      * 1 = material inside

        * 2 = material outside

          * 3 = bend outside

*PCBA*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

Inserts a 3D bend in sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetal3dBend( _    ByVal Angle As System.Double, _    ByVal BUseDefaultRadius As System.Boolean, _    ByVal Radius As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal BendPos As System.Short, _    ByVal PCBA As CustomBendAllowance _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Angle As System.Double Dim BUseDefaultRadius As System.Boolean Dim Radius As System.Double Dim FlipDir As System.Boolean Dim BendPos As System.Short Dim PCBA As CustomBendAllowance Dim value As Feature   value = instance.InsertSheetMetal3dBend(Angle, BUseDefaultRadius, Radius, FlipDir, BendPos, PCBA) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetal3dBend(     System.double Angle,    System.bool BUseDefaultRadius,    System.double Radius,    System.bool FlipDir,    System.short BendPos,    CustomBendAllowance PCBA ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetal3dBend(  &   System.double Angle, &   System.bool BUseDefaultRadius, &   System.double Radius, &   System.bool FlipDir, &   System.short BendPos, &   CustomBendAllowance^ PCBA ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   Angle of the bend in radians

*BUseDefaultRadius*
:   True to use the default radius, false to use the value specified in radius

*Radius*
:   Value for the radius of the bend if bUseDefaultRadius is false

*FlipDir*
:   True to flip the bend direction, false to not

*BendPos*
:   Bend position:

    * 0 = bend centerline

      * 1 = material inside

        * 2 = material outside

          * 3 = bend outside

*PCBA*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetal3dBend.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

[IBendsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0