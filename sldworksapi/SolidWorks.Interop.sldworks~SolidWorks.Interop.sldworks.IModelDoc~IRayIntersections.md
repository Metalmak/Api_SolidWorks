<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~IRayIntersections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IRayIntersections Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : IRayIntersections Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodiesIn*

*NumBodies*

*BasePointsIn*

*VectorsIn*

*NumRays*

*Options*

*HitRadius*

*Offset*

Obsolete. Superseded by [IModelDoc2::IRayIntersections](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IRayIntersections.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IRayIntersections( _    ByRef BodiesIn As Body, _    ByVal NumBodies As System.Integer, _    ByRef BasePointsIn As System.Double, _    ByRef VectorsIn As System.Double, _    ByVal NumRays As System.Integer, _    ByVal Options As System.Integer, _    ByVal HitRadius As System.Double, _    ByVal Offset As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim BodiesIn As Body Dim NumBodies As System.Integer Dim BasePointsIn As System.Double Dim VectorsIn As System.Double Dim NumRays As System.Integer Dim Options As System.Integer Dim HitRadius As System.Double Dim Offset As System.Double Dim value As System.Integer   value = instance.IRayIntersections(BodiesIn, NumBodies, BasePointsIn, VectorsIn, NumRays, Options, HitRadius, Offset) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IRayIntersections(     ref Body BodiesIn,    System.int NumBodies,    ref System.double BasePointsIn,    ref System.double VectorsIn,    System.int NumRays,    System.int Options,    System.double HitRadius,    System.double Offset ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IRayIntersections(  &   Body^% BodiesIn, &   System.int NumBodies, &   System.double% BasePointsIn, &   System.double% VectorsIn, &   System.int NumRays, &   System.int Options, &   System.double HitRadius, &   System.double Offset ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodiesIn*

*NumBodies*

*BasePointsIn*

*VectorsIn*

*NumRays*

*Options*

*HitRadius*

*Offset*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::IRayIntersections.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)