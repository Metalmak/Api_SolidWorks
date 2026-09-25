<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SketchPolygon.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchPolygon Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SketchPolygon Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XCenter*

*YCenter*

*XEdge*

*YEdge*

*NSides*

*BInscribed*

Obsolete. Superseded by [IModelDoc2::SketchPolygon](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SketchPolygon.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchPolygon( _    ByVal XCenter As System.Double, _    ByVal YCenter As System.Double, _    ByVal XEdge As System.Double, _    ByVal YEdge As System.Double, _    ByVal NSides As System.Integer, _    ByVal BInscribed As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim XCenter As System.Double Dim YCenter As System.Double Dim XEdge As System.Double Dim YEdge As System.Double Dim NSides As System.Integer Dim BInscribed As System.Boolean Dim value As System.Boolean   value = instance.SketchPolygon(XCenter, YCenter, XEdge, YEdge, NSides, BInscribed) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchPolygon(     System.double XCenter,    System.double YCenter,    System.double XEdge,    System.double YEdge,    System.int NSides,    System.bool BInscribed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchPolygon(  &   System.double XCenter, &   System.double YCenter, &   System.double XEdge, &   System.double YEdge, &   System.int NSides, &   System.bool BInscribed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XCenter*

*YCenter*

*XEdge*

*YEdge*

*NSides*

*BInscribed*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SketchPolygon.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)