<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~MoveRotateLiveSectionPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoveRotateLiveSectionPlane Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : MoveRotateLiveSectionPlane Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Feat*
:   Name of the Live Section Plane as it appears in the FeatureManager design tree

*Type*
:   * 0 = Move only, then (XorDeltaX, YorDeltaY, and ZorDeltaZ) is delta vector* 1 = Rotate only, then (XorDeltaX, YorDeltaY, and ZorDeltaZ) is the pivot point for rotation, (axisX, axisY, axisZ) is rotating axis

*XorDeltaX*
:   Delta X

*YorDeltaY*
:   Delta Y

*ZorDeltaZ*
:   Delta Z

*Axisx*
:   X axis

*Axisy*
:   Y axis

*Axisz*
:   Z axis

*Angle*
:   Value by to rotate the Live Section Plane

Moves or rotates the selected Live Section Plane using the selected Live Section Plane and its manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MoveRotateLiveSectionPlane( _    ByVal Feat As System.String, _    ByVal Type As System.Short, _    ByVal XorDeltaX As System.Double, _    ByVal YorDeltaY As System.Double, _    ByVal ZorDeltaZ As System.Double, _    ByVal Axisx As System.Double, _    ByVal Axisy As System.Double, _    ByVal Axisz As System.Double, _    ByVal Angle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Feat As System.String Dim Type As System.Short Dim XorDeltaX As System.Double Dim YorDeltaY As System.Double Dim ZorDeltaZ As System.Double Dim Axisx As System.Double Dim Axisy As System.Double Dim Axisz As System.Double Dim Angle As System.Double Dim value As System.Boolean   value = instance.MoveRotateLiveSectionPlane(Feat, Type, XorDeltaX, YorDeltaY, ZorDeltaZ, Axisx, Axisy, Axisz, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MoveRotateLiveSectionPlane(     System.string Feat,    System.short Type,    System.double XorDeltaX,    System.double YorDeltaY,    System.double ZorDeltaZ,    System.double Axisx,    System.double Axisy,    System.double Axisz,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MoveRotateLiveSectionPlane(  &   System.String^ Feat, &   System.short Type, &   System.double XorDeltaX, &   System.double YorDeltaY, &   System.double ZorDeltaZ, &   System.double Axisx, &   System.double Axisy, &   System.double Axisz, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Feat*
:   Name of the Live Section Plane as it appears in the FeatureManager design tree

*Type*
:   * 0 = Move only, then (XorDeltaX, YorDeltaY, and ZorDeltaZ) is delta vector* 1 = Rotate only, then (XorDeltaX, YorDeltaY, and ZorDeltaZ) is the pivot point for rotation, (axisX, axisY, axisZ) is rotating axis

*XorDeltaX*
:   Delta X

*YorDeltaY*
:   Delta Y

*ZorDeltaZ*
:   Delta Z

*Axisx*
:   X axis

*Axisy*
:   Y axis

*Axisz*
:   Z axis

*Angle*
:   Value by to rotate the Live Section Plane

#### Return Value

True if the Live Section Plane moves or rotates, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::MoveRotateLiveSectionPlane.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertLiveSectionPlane Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertLiveSectionPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0