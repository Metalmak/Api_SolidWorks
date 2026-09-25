<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertConvertToSheetMetal2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertConvertToSheetMetal2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertConvertToSheetMetal2 Method (IFeatureManager) |

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

*OverlapType*
:   Overlap type for all rips

    * 1=Open butt* 2=Overlap* 3=Underlap

*OverlapRatio*
:   Overlap ratio for all rips

*KeepBody*
:   True to keep bodies, false to not

Converts a solid or surface body into a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertConvertToSheetMetal2( _    ByVal Thickness As System.Double, _    ByVal ReverseThickDir As System.Boolean, _    ByVal FindBends As System.Boolean, _    ByVal Radius As System.Double, _    ByVal Gap As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal ReliefRatio As System.Double, _    ByVal OverlapType As System.Integer, _    ByVal OverlapRatio As System.Double, _    ByVal KeepBody As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Thickness As System.Double Dim ReverseThickDir As System.Boolean Dim FindBends As System.Boolean Dim Radius As System.Double Dim Gap As System.Double Dim ReliefType As System.Integer Dim ReliefRatio As System.Double Dim OverlapType As System.Integer Dim OverlapRatio As System.Double Dim KeepBody As System.Boolean Dim value As System.Boolean   value = instance.InsertConvertToSheetMetal2(Thickness, ReverseThickDir, FindBends, Radius, Gap, ReliefType, ReliefRatio, OverlapType, OverlapRatio, KeepBody) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertConvertToSheetMetal2(     System.double Thickness,    System.bool ReverseThickDir,    System.bool FindBends,    System.double Radius,    System.double Gap,    System.int ReliefType,    System.double ReliefRatio,    System.int OverlapType,    System.double OverlapRatio,    System.bool KeepBody ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertConvertToSheetMetal2(  &   System.double Thickness, &   System.bool ReverseThickDir, &   System.bool FindBends, &   System.double Radius, &   System.double Gap, &   System.int ReliefType, &   System.double ReliefRatio, &   System.int OverlapType, &   System.double OverlapRatio, &   System.bool KeepBody ) ``` | |

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

*OverlapType*
:   Overlap type for all rips

    * 1=Open butt* 2=Overlap* 3=Underlap

*OverlapRatio*
:   Overlap ratio for all rips

*KeepBody*
:   True to keep bodies, false to not

#### Return Value

True if a Convert-Solid sheet metal feature is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertConvertToSheetMetal2.

# ![](dotnetimages/collapse.gif)Example

[Convert Extrusion to Sheet Metal (C#)](Insert_Convert_to_Sheet_Metal_Example_CSharp.htm)

[Convert Extrusion to Sheet Metal (VB.NET)](Insert_Convert_to_Sheet_Metal_Example_VBNET.htm)

[Convert Extrusion to Sheet Metal (VBA)](Insert_Convert_to_Sheet_Metal_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Read the SOLIDWORKS Help to learn more about converting to sheet metal.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0