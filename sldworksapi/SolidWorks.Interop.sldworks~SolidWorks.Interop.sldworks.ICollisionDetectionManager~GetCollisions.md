<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager~GetCollisions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCollisions Method (ICollisionDetectionManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICollisionDetectionManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html) : GetCollisions Method (ICollisionDetectionManager) |

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

*Collisions*
:   Array of [ICollision](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html)s

Gets the collisions detected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCollisions( _    ByVal TreatContactAsCollision As System.Boolean, _    ByRef Collisions As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICollisionDetectionManager Dim TreatContactAsCollision As System.Boolean Dim Collisions As System.Object Dim value As System.Integer   value = instance.GetCollisions(TreatContactAsCollision, Collisions) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCollisions(     System.bool TreatContactAsCollision,    out System.object Collisions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCollisions(  &   System.bool TreatContactAsCollision, &   [Out] System.Object^ Collisions ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TreatContactAsCollision*
:   True to treat touching faces/edges/vertices as colliding, false to require solid bodies to overlap in a finite volume

*Collisions*
:   Array of [ICollision](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html)s

#### Return Value

Number of collisions found

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CollisionDetectionManager::GetCollisions.

# ![](dotnetimages/collapse.gif)Example

See the [ICollisionDetectionManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Use [ICollisionDetectionManager::IsCollisionPresent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager~IsCollisionPresent.html) to determine whether to run this method.

This method can take significantly longer to execute than ICollisionDetectionManager::IsCollisionPresent, because this method might perform the collision detection calculation repeatedly.

# ![](dotnetimages/collapse.gif)See Also

####

[ICollisionDetectionManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html)

[ICollisionDetectionManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0