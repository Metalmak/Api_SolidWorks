<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SetGridOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetGridOptions Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SetGridOptions Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Display*
:   True to display the grid, false if not

*Spacing*
:   Snap distance

*Snap*
:   True to snap to grid, false to not

*DotStyle*
:   True for dotted grids, false if not

*NumMajor*
:   Number of minors in major

*NumMinor*
:   Number of snaps in minor

*AlignToEdge*
:   True if to align to an edge, false if not

*AngleSnap*
:   True to snap to angle, false to not

*AngleUnit*
:   Angle at which to snap

*MinorAuto*
:   True if the minor grids are to be set automatically, false if not

Sets the options for the grid.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetGridOptions( _    ByVal Display As System.Boolean, _    ByVal Spacing As System.Double, _    ByVal Snap As System.Boolean, _    ByVal DotStyle As System.Boolean, _    ByVal NumMajor As System.Short, _    ByVal NumMinor As System.Short, _    ByVal AlignToEdge As System.Boolean, _    ByVal AngleSnap As System.Boolean, _    ByVal AngleUnit As System.Double, _    ByVal MinorAuto As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Display As System.Boolean Dim Spacing As System.Double Dim Snap As System.Boolean Dim DotStyle As System.Boolean Dim NumMajor As System.Short Dim NumMinor As System.Short Dim AlignToEdge As System.Boolean Dim AngleSnap As System.Boolean Dim AngleUnit As System.Double Dim MinorAuto As System.Boolean   instance.SetGridOptions(Display, Spacing, Snap, DotStyle, NumMajor, NumMinor, AlignToEdge, AngleSnap, AngleUnit, MinorAuto) ``` | |

| C# |  |
| --- | --- |
| ``` void SetGridOptions(     System.bool Display,    System.double Spacing,    System.bool Snap,    System.bool DotStyle,    System.short NumMajor,    System.short NumMinor,    System.bool AlignToEdge,    System.bool AngleSnap,    System.double AngleUnit,    System.bool MinorAuto ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetGridOptions(  &   System.bool Display, &   System.double Spacing, &   System.bool Snap, &   System.bool DotStyle, &   System.short NumMajor, &   System.short NumMinor, &   System.bool AlignToEdge, &   System.bool AngleSnap, &   System.double AngleUnit, &   System.bool MinorAuto ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Display*
:   True to display the grid, false if not

*Spacing*
:   Snap distance

*Snap*
:   True to snap to grid, false to not

*DotStyle*
:   True for dotted grids, false if not

*NumMajor*
:   Number of minors in major

*NumMinor*
:   Number of snaps in minor

*AlignToEdge*
:   True if to align to an edge, false if not

*AngleSnap*
:   True to snap to angle, false to not

*AngleUnit*
:   Angle at which to snap

*MinorAuto*
:   True if the minor grids are to be set automatically, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SetGridOptions.

# ![](dotnetimages/collapse.gif)Remarks

The AlignToEdge argument aligns the grid with the currently selected edge. If AlignToEdge is set to TRUE, then you must have selected an edge.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0