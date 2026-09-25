<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~GridOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GridOptions Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : GridOptions Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispGrid*

*GridSpacing*

*Snap*

*DotStyle*

*NMajor*

*NMinor*

*Align2edge*

*AngleSnap*

*AngleUnit*

*MinorAuto*

Obsolete. Superseded by [IModelDoc2::GridOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GridOptions.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GridOptions( _    ByVal DispGrid As System.Boolean, _    ByVal GridSpacing As System.Double, _    ByVal Snap As System.Boolean, _    ByVal DotStyle As System.Boolean, _    ByVal NMajor As System.Short, _    ByVal NMinor As System.Short, _    ByVal Align2edge As System.Boolean, _    ByVal AngleSnap As System.Boolean, _    ByVal AngleUnit As System.Double, _    ByVal MinorAuto As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim DispGrid As System.Boolean Dim GridSpacing As System.Double Dim Snap As System.Boolean Dim DotStyle As System.Boolean Dim NMajor As System.Short Dim NMinor As System.Short Dim Align2edge As System.Boolean Dim AngleSnap As System.Boolean Dim AngleUnit As System.Double Dim MinorAuto As System.Boolean   instance.GridOptions(DispGrid, GridSpacing, Snap, DotStyle, NMajor, NMinor, Align2edge, AngleSnap, AngleUnit, MinorAuto) ``` | |

| C# |  |
| --- | --- |
| ``` void GridOptions(     System.bool DispGrid,    System.double GridSpacing,    System.bool Snap,    System.bool DotStyle,    System.short NMajor,    System.short NMinor,    System.bool Align2edge,    System.bool AngleSnap,    System.double AngleUnit,    System.bool MinorAuto ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GridOptions(  &   System.bool DispGrid, &   System.double GridSpacing, &   System.bool Snap, &   System.bool DotStyle, &   System.short NMajor, &   System.short NMinor, &   System.bool Align2edge, &   System.bool AngleSnap, &   System.double AngleUnit, &   System.bool MinorAuto ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DispGrid*

*GridSpacing*

*Snap*

*DotStyle*

*NMajor*

*NMinor*

*Align2edge*

*AngleSnap*

*AngleUnit*

*MinorAuto*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::GridOptions.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)