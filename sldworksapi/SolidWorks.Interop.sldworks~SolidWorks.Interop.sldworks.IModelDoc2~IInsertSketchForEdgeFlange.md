<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IInsertSketchForEdgeFlange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertSketchForEdgeFlange Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IInsertSketchForEdgeFlange Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FlangeEdge*
:   Edge to which to apply flange

*DAngle*
:   Angle of flange

*FlipDir*
:   True reverses the offset direction of the flange, false does not

Inserts a sketch for [IFeatureManager::InsertSheetMetalEdgeFlange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertSheetMetalEdgeFlange2.html) in this sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertSketchForEdgeFlange( _    ByVal FlangeEdge As Edge, _    ByVal DAngle As System.Double, _    ByVal FlipDir As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim FlangeEdge As Edge Dim DAngle As System.Double Dim FlipDir As System.Boolean Dim value As Feature   value = instance.IInsertSketchForEdgeFlange(FlangeEdge, DAngle, FlipDir) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertSketchForEdgeFlange(     Edge FlangeEdge,    System.double DAngle,    System.bool FlipDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertSketchForEdgeFlange(  &   Edge^ FlangeEdge, &   System.double DAngle, &   System.bool FlipDir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FlangeEdge*
:   Edge to which to apply flange

*DAngle*
:   Angle of flange

*FlipDir*
:   True reverses the offset direction of the flange, false does not

#### Return Value

Sketch for the edge flagne, returned as a [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IInsertSketchForEdgeFlange.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must create the profile for the flange on the appropriate plane. After creating the profile, call [IFeatureManager::InsertSheetMetalEdgeFlange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertSheetMetalEdgeFlange2.html) to create the flange.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::InsertSheetMetalMiterFlange Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSheetMetalMiterFlange.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0