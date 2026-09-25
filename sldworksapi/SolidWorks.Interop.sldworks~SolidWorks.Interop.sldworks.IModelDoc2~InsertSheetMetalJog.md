<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSheetMetalJog.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalJog Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertSheetMetalJog Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   Jog angle

*Radius*
:   Jog radius

*OffsetDist*
:   Offset distance

*FlipDir*
:   True flips the jog direction, false does not

*FixProjLen*
:   True fixes the projected length, false does not

*DimPos*
:   Dimension position

*BendPos*
:   Bend position

Inserts a sheet metal jog in the current model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertSheetMetalJog( _    ByVal Angle As System.Double, _    ByVal Radius As System.Double, _    ByVal OffsetDist As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal FixProjLen As System.Boolean, _    ByVal DimPos As System.Short, _    ByVal BendPos As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Angle As System.Double Dim Radius As System.Double Dim OffsetDist As System.Double Dim FlipDir As System.Boolean Dim FixProjLen As System.Boolean Dim DimPos As System.Short Dim BendPos As System.Short   instance.InsertSheetMetalJog(Angle, Radius, OffsetDist, FlipDir, FixProjLen, DimPos, BendPos) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertSheetMetalJog(     System.double Angle,    System.double Radius,    System.double OffsetDist,    System.bool FlipDir,    System.bool FixProjLen,    System.short DimPos,    System.short BendPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertSheetMetalJog(  &   System.double Angle, &   System.double Radius, &   System.double OffsetDist, &   System.bool FlipDir, &   System.bool FixProjLen, &   System.short DimPos, &   System.short BendPos ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   Jog angle

*Radius*
:   Jog radius

*OffsetDist*
:   Offset distance

*FlipDir*
:   True flips the jog direction, false does not

*FixProjLen*
:   True fixes the projected length, false does not

*DimPos*
:   Dimension position

*BendPos*
:   Bend position

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertSheetMetalJog.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IJogFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IJogFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0