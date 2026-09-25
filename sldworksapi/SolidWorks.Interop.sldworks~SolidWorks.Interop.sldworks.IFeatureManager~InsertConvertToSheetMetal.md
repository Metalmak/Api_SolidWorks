<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertConvertToSheetMetal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertConvertToSheetMetal Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertConvertToSheetMetal Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Thickness*
:   Sheet thickness

*ReverseThickDir*
:   True to reverse the direction of the sheet thickness, false to not

*FindBends*
:   True to find pre-made bends and part thickness, false to not

*Radius*
:   Radius for the bends

*Gap*
:   Gap for all rips

*ReliefType*
:   Relief type as defined by swSheetMetalReliefTypes\_e

*ReliefRatio*
:   Relief ratio

Obsolete. Superseded by [IFeatureManager::InsertConvertToSheetMetal2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertConvertToSheetMetal2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertConvertToSheetMetal( _    ByVal Thickness As System.Double, _    ByVal ReverseThickDir As System.Boolean, _    ByVal FindBends As System.Boolean, _    ByVal Radius As System.Double, _    ByVal Gap As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal ReliefRatio As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Thickness As System.Double Dim ReverseThickDir As System.Boolean Dim FindBends As System.Boolean Dim Radius As System.Double Dim Gap As System.Double Dim ReliefType As System.Integer Dim ReliefRatio As System.Double Dim value As System.Boolean   value = instance.InsertConvertToSheetMetal(Thickness, ReverseThickDir, FindBends, Radius, Gap, ReliefType, ReliefRatio) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertConvertToSheetMetal(     System.double Thickness,    System.bool ReverseThickDir,    System.bool FindBends,    System.double Radius,    System.double Gap,    System.int ReliefType,    System.double ReliefRatio ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertConvertToSheetMetal(  &   System.double Thickness, &   System.bool ReverseThickDir, &   System.bool FindBends, &   System.double Radius, &   System.double Gap, &   System.int ReliefType, &   System.double ReliefRatio ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*
:   Sheet thickness

*ReverseThickDir*
:   True to reverse the direction of the sheet thickness, false to not

*FindBends*
:   True to find pre-made bends and part thickness, false to not

*Radius*
:   Radius for the bends

*Gap*
:   Gap for all rips

*ReliefType*
:   Relief type as defined by swSheetMetalReliefTypes\_e

*ReliefRatio*
:   Relief ratio

#### Return Value

True if a Convert-Solid sheet metal feature is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertConvertToSheetMetal.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SolidwWorks 2009 FCS, Revision Number 17.0