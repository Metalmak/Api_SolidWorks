<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalHem2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalHem2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetalHem2 Method (IFeatureManager) |

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

*UseDefaultRelief*
:   True to use the default relief, false to use the relief specified by ReliefType

*ReliefType*
:   Type of relief as defined in swSheetMetalReliefTypes\_e; valid only if UseDefaultRelief is false

*ReliefTearTypes*
:   Type of relief tear as defined in  swReliefTearTypes\_e; valid only when:

    * UseDefaultRelief is false

        - and -

    * ReliefType is swSheetMetalReliefTypes\_e.swSheetMetalReliefTear

*UseReliefRatio*
:   True to use ReliefRatio, false to use ReliefWidth/ReliefDepth; valid only when:

    * UseDefaultRelief is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefRatio*
:   Relief ratio; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is true

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefWidth*
:   Width of the relief; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefDepth*
:   Depth of the relief; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

Inserts a hem of the specified relief type at the selected edges of the current sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetalHem2( _    ByVal Type As System.Integer, _    ByVal Position As System.Integer, _    ByVal Reverse As System.Boolean, _    ByVal DLength As System.Double, _    ByVal DGap As System.Double, _    ByVal DAngle As System.Double, _    ByVal DRad As System.Double, _    ByVal DMiterGap As System.Double, _    ByVal PCBA As CustomBendAllowance, _    ByVal UseDefaultRelief As System.Boolean, _    ByVal ReliefType As System.Integer, _    ByVal ReliefTearTypes As System.Integer, _    ByVal UseReliefRatio As System.Boolean, _    ByVal ReliefRatio As System.Double, _    ByVal ReliefWidth As System.Double, _    ByVal ReliefDepth As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim Position As System.Integer Dim Reverse As System.Boolean Dim DLength As System.Double Dim DGap As System.Double Dim DAngle As System.Double Dim DRad As System.Double Dim DMiterGap As System.Double Dim PCBA As CustomBendAllowance Dim UseDefaultRelief As System.Boolean Dim ReliefType As System.Integer Dim ReliefTearTypes As System.Integer Dim UseReliefRatio As System.Boolean Dim ReliefRatio As System.Double Dim ReliefWidth As System.Double Dim ReliefDepth As System.Double Dim value As Feature   value = instance.InsertSheetMetalHem2(Type, Position, Reverse, DLength, DGap, DAngle, DRad, DMiterGap, PCBA, UseDefaultRelief, ReliefType, ReliefTearTypes, UseReliefRatio, ReliefRatio, ReliefWidth, ReliefDepth) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetalHem2(     System.int Type,    System.int Position,    System.bool Reverse,    System.double DLength,    System.double DGap,    System.double DAngle,    System.double DRad,    System.double DMiterGap,    CustomBendAllowance PCBA,    System.bool UseDefaultRelief,    System.int ReliefType,    System.int ReliefTearTypes,    System.bool UseReliefRatio,    System.double ReliefRatio,    System.double ReliefWidth,    System.double ReliefDepth ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetalHem2(  &   System.int Type, &   System.int Position, &   System.bool Reverse, &   System.double DLength, &   System.double DGap, &   System.double DAngle, &   System.double DRad, &   System.double DMiterGap, &   CustomBendAllowance^ PCBA, &   System.bool UseDefaultRelief, &   System.int ReliefType, &   System.int ReliefTearTypes, &   System.bool UseReliefRatio, &   System.double ReliefRatio, &   System.double ReliefWidth, &   System.double ReliefDepth ) ``` | |

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

*UseDefaultRelief*
:   True to use the default relief, false to use the relief specified by ReliefType

*ReliefType*
:   Type of relief as defined in swSheetMetalReliefTypes\_e; valid only if UseDefaultRelief is false

*ReliefTearTypes*
:   Type of relief tear as defined in  swReliefTearTypes\_e; valid only when:

    * UseDefaultRelief is false

        - and -

    * ReliefType is swSheetMetalReliefTypes\_e.swSheetMetalReliefTear

*UseReliefRatio*
:   True to use ReliefRatio, false to use ReliefWidth/ReliefDepth; valid only when:

    * UseDefaultRelief is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefRatio*
:   Relief ratio; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is true

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefWidth*
:   Width of the relief; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

*ReliefDepth*
:   Depth of the relief; valid only when:

    * UseDefaultRelief is false

        - and -

    * UseReliefRatio is false

        - and -

    * ReliefType is either swSheetMetalReliefTypes\_e.swSheetMetalReliefObround or swSheetMetalReliefTypes\_e.swSheetMetalReliefRectangular

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetalHem2.

# ![](dotnetimages/collapse.gif)Example

[Insert Sheet Metal Hem (VBA)](Insert_Sheet_Metal_Hem_Example_VB.htm)

[Insert Sheet Metal Hem (VB.NET)](Insert_Sheet_Metal_Hem_Example_VBNET.htm)

[Insert Sheet Metal Hem (C#)](Insert_Sheet_Metal_Hem_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. Call [IFeatureManager::CreateCustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~CreateCustomBendAllowance.html) to create an instance of ICustomBendAllowance.- Initialize the CustomBendAllowance object.- Assign PCBA to the initialized CustomBendAllowance object.- Select one or more edges in the sheet metal model to which to add the specified hem.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IHemFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHemFeatureData.html)

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP03, Revision Number 19.3