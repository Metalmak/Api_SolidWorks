<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureChamferType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureChamferType Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureChamferType Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ChamferType*

*Width*

*Angle*

*Flip*

*OtherDist*

*VertexChamDist1*

*VertexChamDist2*

*VertexChamDist3*

Obsolete. Superseded by [IFeatureManager::InsertFeatureChamfer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertFeatureChamfer.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub FeatureChamferType( _    ByVal ChamferType As System.Short, _    ByVal Width As System.Double, _    ByVal Angle As System.Double, _    ByVal Flip As System.Boolean, _    ByVal OtherDist As System.Double, _    ByVal VertexChamDist1 As System.Double, _    ByVal VertexChamDist2 As System.Double, _    ByVal VertexChamDist3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ChamferType As System.Short Dim Width As System.Double Dim Angle As System.Double Dim Flip As System.Boolean Dim OtherDist As System.Double Dim VertexChamDist1 As System.Double Dim VertexChamDist2 As System.Double Dim VertexChamDist3 As System.Double   instance.FeatureChamferType(ChamferType, Width, Angle, Flip, OtherDist, VertexChamDist1, VertexChamDist2, VertexChamDist3) ``` | |

| C# |  |
| --- | --- |
| ``` void FeatureChamferType(     System.short ChamferType,    System.double Width,    System.double Angle,    System.bool Flip,    System.double OtherDist,    System.double VertexChamDist1,    System.double VertexChamDist2,    System.double VertexChamDist3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void FeatureChamferType(  &   System.short ChamferType, &   System.double Width, &   System.double Angle, &   System.bool Flip, &   System.double OtherDist, &   System.double VertexChamDist1, &   System.double VertexChamDist2, &   System.double VertexChamDist3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ChamferType*

*Width*

*Angle*

*Flip*

*OtherDist*

*VertexChamDist1*

*VertexChamDist2*

*VertexChamDist3*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureChamferType.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)