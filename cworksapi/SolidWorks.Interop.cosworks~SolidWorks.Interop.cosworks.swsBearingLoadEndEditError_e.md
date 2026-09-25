<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsBearingLoadEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsBearingLoadEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsBearingLoadEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Bearing load editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsBearingLoadEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsBearingLoadEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsBearingLoadEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsBearingLoadEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsBearingLoadEndEditErrorBodyExcludedFromAnalysis** | 17 = Selected entity is on a body excluded from analysis |
| **swsBearingLoadEndEditErrorCoordinateSystemCylindricalFaces** | 1 = Coordinate system and set of cylindrical faces must be the same radii and z axis of coordinate system must be coincident with the axis of the cylindrical faces |
| **swsBearingLoadEndEditErrorEntityExists** | 3 = Entity already exists |
| **swsBearingLoadEndEditErrorHasBeamBody** | 9 = Bearing load has a beam body |
| **swsBearingLoadEndEditErrorHasMassElement** | 8 = Bearing load has a mass element |
| **swsBearingLoadEndEditErrorIncorrectOrNullEntity** | 2 = Incorrect or NULL entity |
| **swsBearingLoadEndEditErrorIndexExceedsNumberOfEntities** | 10 = Specified index exceeds the number of entities |
| **swsBearingLoadEndEditErrorNoEntity** | 11 = No entity |
| **swsBearingLoadEndEditErrorNoEntityAtIndex** | 5 = No entity at specified index |
| **swsBearingLoadEndEditErrorNullEntity** | 16 = Entity is NULL |
| **swsBearingLoadEndEditErrorSelectFace** | 4 = Select a face |
| **swsBearingLoadEndEditErrorSelectFaceWithCylindricalSurface** | 7 = Select a face with cylindrical surface |
| **swsBearingLoadEndEditErrorSelectForceDirection** | 13 = Select one force direction |
| **swsBearingLoadEndEditErrorSelectOneForceDirection** | 12 = Select one force direction, not both force directions |
| **swsBearingLoadEndEditErrorSetXDirection** | 14 = Set X direction to 0 or 1 |
| **swsBearingLoadEndEditErrorSetYDirection** | 15 = Set Y direction to 0 or 1 |
| **swsBearingLoadEndEditErrorSpecifyValue** | 6 = Specify a value > 0 |
| **swsBearingLoadEndEditErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)