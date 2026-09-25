<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalCornerTrim.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalCornerTrim Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetalCornerTrim Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InternalCornerFlag*
:   Do internal corners only

*BreakType*
:   Type of break as defined in swBreakCornerTypes\_e

*BreakDist*
:   Distance to break from corner

*ReliefType*
:   Type of relief:

    * 0 = circular

      * 1 = square

        * 2 = bend-waist

*Param*
:   ReliefType dependent:

    * circular, its diameter

      * square, its side length

        * bend-waist, its radius

Inserts a break corner trim in the sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetalCornerTrim( _    ByVal InternalCornerFlag As System.Integer, _    ByVal BreakType As System.Integer, _    ByVal BreakDist As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal Param As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim InternalCornerFlag As System.Integer Dim BreakType As System.Integer Dim BreakDist As System.Double Dim ReliefType As System.Integer Dim Param As System.Double Dim value As Feature   value = instance.InsertSheetMetalCornerTrim(InternalCornerFlag, BreakType, BreakDist, ReliefType, Param) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetalCornerTrim(     System.int InternalCornerFlag,    System.int BreakType,    System.double BreakDist,    System.int ReliefType,    System.double Param ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetalCornerTrim(  &   System.int InternalCornerFlag, &   System.int BreakType, &   System.double BreakDist, &   System.int ReliefType, &   System.double Param ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InternalCornerFlag*
:   Do internal corners only

*BreakType*
:   Type of break as defined in swBreakCornerTypes\_e

*BreakDist*
:   Distance to break from corner

*ReliefType*
:   Type of relief:

    * 0 = circular

      * 1 = square

        * 2 = bend-waist

*Param*
:   ReliefType dependent:

    * circular, its diameter

      * square, its side length

        * bend-waist, its radius

#### Return Value

Pointer to the break corner trim [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) in the sheet metal part

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetalCornerTrim.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IBreakCornerFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData.html)

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0