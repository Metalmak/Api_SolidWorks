<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager~IsCollisionPresent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsCollisionPresent Method (ICollisionDetectionManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICollisionDetectionManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html) : IsCollisionPresent Method (ICollisionDetectionManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TreatContactAsCollision*
:   True to treat touching faces/edges/vertices as colliding, false to require solid bodies to overlap in a finite volume

Performs collision detection analysis between all groups of components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsCollisionPresent( _    ByVal TreatContactAsCollision As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICollisionDetectionManager Dim TreatContactAsCollision As System.Boolean Dim value As System.Integer   value = instance.IsCollisionPresent(TreatContactAsCollision) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IsCollisionPresent(     System.bool TreatContactAsCollision ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IsCollisionPresent(  &   System.bool TreatContactAsCollision ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TreatContactAsCollision*
:   True to treat touching faces/edges/vertices as colliding, false to require solid bodies to overlap in a finite volume

#### Return Value

Return code as defined in swCollisionDetectionResults\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CollisionDetectionManager::IsCollisionPresent.

# ![](dotnetimages/collapse.gif)Example

See the [ICollisionDetectionManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method takes less time to run than [ICollisionDetectionManager::GetCollisions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager~GetCollisions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICollisionDetectionManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html)

[ICollisionDetectionManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0