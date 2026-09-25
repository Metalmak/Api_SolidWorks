<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchChamfer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchChamfer Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchChamfer Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AngleORdist*
:   Angle of the chamfer if using the Angle-Distance option or the distance of the second distance if using the Distance-Distance option

*Dist1*
:   Distance of the chamfer

*Options*
:   0 = Angle - Distance Chamfer

    1 = Distance - Distance Chamfer

Obsolete. Superseded by [ISketchManager::CreateChamfer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateChamfer.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchChamfer( _    ByVal AngleORdist As System.Double, _    ByVal Dist1 As System.Double, _    ByVal Options As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim AngleORdist As System.Double Dim Dist1 As System.Double Dim Options As System.Integer   instance.SketchChamfer(AngleORdist, Dist1, Options) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchChamfer(     System.double AngleORdist,    System.double Dist1,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchChamfer(  &   System.double AngleORdist, &   System.double Dist1, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AngleORdist*
:   Angle of the chamfer if using the Angle-Distance option or the distance of the second distance if using the Distance-Distance option

*Dist1*
:   Distance of the chamfer

*Options*
:   0 = Angle - Distance Chamfer

    1 = Distance - Distance Chamfer

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchChamfer.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0