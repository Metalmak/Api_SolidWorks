<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertRuledSurfaceFromEdge.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRuledSurfaceFromEdge Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertRuledSurfaceFromEdge Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*

*Length*

*FlipPullDir*

*FlipDir*

*TrimAndSew*

*Angle*

*CoordInput*

*X*

*Y*

*Z*

Obsolete. Superseded by [IFeatureManager::InsertRuledSurfaceFromEdge2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertRuledSurfaceFromEdge2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRuledSurfaceFromEdge( _    ByVal Type As System.Integer, _    ByVal Length As System.Double, _    ByVal FlipPullDir As System.Boolean, _    ByVal FlipDir As System.Boolean, _    ByVal TrimAndSew As System.Boolean, _    ByVal Angle As System.Double, _    ByVal CoordInput As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim Length As System.Double Dim FlipPullDir As System.Boolean Dim FlipDir As System.Boolean Dim TrimAndSew As System.Boolean Dim Angle As System.Double Dim CoordInput As System.Boolean Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As Feature   value = instance.InsertRuledSurfaceFromEdge(Type, Length, FlipPullDir, FlipDir, TrimAndSew, Angle, CoordInput, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertRuledSurfaceFromEdge(     System.int Type,    System.double Length,    System.bool FlipPullDir,    System.bool FlipDir,    System.bool TrimAndSew,    System.double Angle,    System.bool CoordInput,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertRuledSurfaceFromEdge(  &   System.int Type, &   System.double Length, &   System.bool FlipPullDir, &   System.bool FlipDir, &   System.bool TrimAndSew, &   System.double Angle, &   System.bool CoordInput, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*

*Length*

*FlipPullDir*

*FlipDir*

*TrimAndSew*

*Angle*

*CoordInput*

*X*

*Y*

*Z*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertRuledSurfaceFromEdge.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)