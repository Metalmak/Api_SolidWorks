<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~RayIntersections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RayIntersections Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : RayIntersections Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodiesIn*

*BasePointsIn*

*VectorsIn*

*Options*

*HitRadius*

*Offset*

Obsolete. Superseded by [IModelDoc2::RayIntersections](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~RayIntersections.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RayIntersections( _    ByVal BodiesIn As System.Object, _    ByVal BasePointsIn As System.Object, _    ByVal VectorsIn As System.Object, _    ByVal Options As System.Integer, _    ByVal HitRadius As System.Double, _    ByVal Offset As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim BodiesIn As System.Object Dim BasePointsIn As System.Object Dim VectorsIn As System.Object Dim Options As System.Integer Dim HitRadius As System.Double Dim Offset As System.Double Dim value As System.Integer   value = instance.RayIntersections(BodiesIn, BasePointsIn, VectorsIn, Options, HitRadius, Offset) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RayIntersections(     System.object BodiesIn,    System.object BasePointsIn,    System.object VectorsIn,    System.int Options,    System.double HitRadius,    System.double Offset ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RayIntersections(  &   System.Object^ BodiesIn, &   System.Object^ BasePointsIn, &   System.Object^ VectorsIn, &   System.int Options, &   System.double HitRadius, &   System.double Offset ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodiesIn*

*BasePointsIn*

*VectorsIn*

*Options*

*HitRadius*

*Offset*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::RayIntersections.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)