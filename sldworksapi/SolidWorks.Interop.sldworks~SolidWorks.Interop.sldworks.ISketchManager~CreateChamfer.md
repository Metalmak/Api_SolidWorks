<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateChamfer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateChamfer Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateChamfer Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of chamfer as defined in swSketchChamferType\_e

*Distance*
:   Distance of the chamfer

*AngleORdist*
:   * If Type = swSketchChamfer\_DistanceDistance, then the second chamfer distance* If Type = swSketchChamfer\_DistanceAngle, then the second chamfer angle* If Type = swSketchChamfer\_DistanceEqual, then this argument is ignored because Distance
          is used for both edges

Creates a chamfer between two selected sketch entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateChamfer( _    ByVal Type As System.Integer, _    ByVal Distance As System.Double, _    ByVal AngleORdist As System.Double _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Type As System.Integer Dim Distance As System.Double Dim AngleORdist As System.Double Dim value As SketchSegment   value = instance.CreateChamfer(Type, Distance, AngleORdist) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment CreateChamfer(     System.int Type,    System.double Distance,    System.double AngleORdist ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ CreateChamfer(  &   System.int Type, &   System.double Distance, &   System.double AngleORdist ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type of chamfer as defined in swSketchChamferType\_e

*Distance*
:   Distance of the chamfer

*AngleORdist*
:   * If Type = swSketchChamfer\_DistanceDistance, then the second chamfer distance* If Type = swSketchChamfer\_DistanceAngle, then the second chamfer angle* If Type = swSketchChamfer\_DistanceEqual, then this argument is ignored because Distance
          is used for both edges

#### Return Value

[Sketch segment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) for the chamfer

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateChamfer.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0