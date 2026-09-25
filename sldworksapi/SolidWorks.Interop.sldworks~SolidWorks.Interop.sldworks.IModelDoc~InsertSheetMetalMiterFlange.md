<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertSheetMetalMiterFlange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalMiterFlange Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertSheetMetalMiterFlange Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseReliefRatio*

*UseDefaultGap*

*UseAutoRelief*

*GlobalRadius*

*RipGap*

*AutoReliefRatio*

*AutoReliefWidth*

*AutoReliefDepth*

*ReliefType*

*RipLocation*

*TrimSideBends*

Obsolete. Superseded by [IModelDoc2::InsertSheetMetalMiterFlange](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertSheetMetalMiterFlange.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertSheetMetalMiterFlange( _    ByVal UseReliefRatio As System.Boolean, _    ByVal UseDefaultGap As System.Boolean, _    ByVal UseAutoRelief As System.Boolean, _    ByVal GlobalRadius As System.Double, _    ByVal RipGap As System.Double, _    ByVal AutoReliefRatio As System.Double, _    ByVal AutoReliefWidth As System.Double, _    ByVal AutoReliefDepth As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal RipLocation As System.Integer, _    ByVal TrimSideBends As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim UseReliefRatio As System.Boolean Dim UseDefaultGap As System.Boolean Dim UseAutoRelief As System.Boolean Dim GlobalRadius As System.Double Dim RipGap As System.Double Dim AutoReliefRatio As System.Double Dim AutoReliefWidth As System.Double Dim AutoReliefDepth As System.Double Dim ReliefType As System.Integer Dim RipLocation As System.Integer Dim TrimSideBends As System.Boolean   instance.InsertSheetMetalMiterFlange(UseReliefRatio, UseDefaultGap, UseAutoRelief, GlobalRadius, RipGap, AutoReliefRatio, AutoReliefWidth, AutoReliefDepth, ReliefType, RipLocation, TrimSideBends) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertSheetMetalMiterFlange(     System.bool UseReliefRatio,    System.bool UseDefaultGap,    System.bool UseAutoRelief,    System.double GlobalRadius,    System.double RipGap,    System.double AutoReliefRatio,    System.double AutoReliefWidth,    System.double AutoReliefDepth,    System.int ReliefType,    System.int RipLocation,    System.bool TrimSideBends ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertSheetMetalMiterFlange(  &   System.bool UseReliefRatio, &   System.bool UseDefaultGap, &   System.bool UseAutoRelief, &   System.double GlobalRadius, &   System.double RipGap, &   System.double AutoReliefRatio, &   System.double AutoReliefWidth, &   System.double AutoReliefDepth, &   System.int ReliefType, &   System.int RipLocation, &   System.bool TrimSideBends ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseReliefRatio*

*UseDefaultGap*

*UseAutoRelief*

*GlobalRadius*

*RipGap*

*AutoReliefRatio*

*AutoReliefWidth*

*AutoReliefDepth*

*ReliefType*

*RipLocation*

*TrimSideBends*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertSheetMetalMiterFlange.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)