<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GridOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GridOptions Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : GridOptions Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispGrid*
:   True to display the grid, false to not

*GridSpacing*
:   Snap distance

*Snap*
:   True to snap to grid, false to not

*DotStyle*
:   True for dotted grids, false for not

*NMajor*
:   Number of minors in major

*NMinor*
:   Number of snaps in minor

*Align2edge*
:   True if to align to an edge, false to not

*AngleSnap*
:   True to snap to angle, false to not

*AngleUnit*
:   Value of angle to which to snap

*MinorAuto*
:   True if the minor grids are to be set automatically, false if not

Obsolete. Superseded by [ISketchManager::SetGridOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~SetGridOptions.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GridOptions( _    ByVal DispGrid As System.Boolean, _    ByVal GridSpacing As System.Double, _    ByVal Snap As System.Boolean, _    ByVal DotStyle As System.Boolean, _    ByVal NMajor As System.Short, _    ByVal NMinor As System.Short, _    ByVal Align2edge As System.Boolean, _    ByVal AngleSnap As System.Boolean, _    ByVal AngleUnit As System.Double, _    ByVal MinorAuto As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim DispGrid As System.Boolean Dim GridSpacing As System.Double Dim Snap As System.Boolean Dim DotStyle As System.Boolean Dim NMajor As System.Short Dim NMinor As System.Short Dim Align2edge As System.Boolean Dim AngleSnap As System.Boolean Dim AngleUnit As System.Double Dim MinorAuto As System.Boolean   instance.GridOptions(DispGrid, GridSpacing, Snap, DotStyle, NMajor, NMinor, Align2edge, AngleSnap, AngleUnit, MinorAuto) ``` | |

| C# |  |
| --- | --- |
| ``` void GridOptions(     System.bool DispGrid,    System.double GridSpacing,    System.bool Snap,    System.bool DotStyle,    System.short NMajor,    System.short NMinor,    System.bool Align2edge,    System.bool AngleSnap,    System.double AngleUnit,    System.bool MinorAuto ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GridOptions(  &   System.bool DispGrid, &   System.double GridSpacing, &   System.bool Snap, &   System.bool DotStyle, &   System.short NMajor, &   System.short NMinor, &   System.bool Align2edge, &   System.bool AngleSnap, &   System.double AngleUnit, &   System.bool MinorAuto ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DispGrid*
:   True to display the grid, false to not

*GridSpacing*
:   Snap distance

*Snap*
:   True to snap to grid, false to not

*DotStyle*
:   True for dotted grids, false for not

*NMajor*
:   Number of minors in major

*NMinor*
:   Number of snaps in minor

*Align2edge*
:   True if to align to an edge, false to not

*AngleSnap*
:   True to snap to angle, false to not

*AngleUnit*
:   Value of angle to which to snap

*MinorAuto*
:   True if the minor grids are to be set automatically, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::GridOptions.

# ![](dotnetimages/collapse.gif)Remarks

The Align2edge argument aligns the grid with the currently selected edge. If Align2edge is set to True, then you must have selected an edge.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetGridSettings Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetGridSettings.html)

[IModelDoc2::ToolsGrid Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ToolsGrid.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0