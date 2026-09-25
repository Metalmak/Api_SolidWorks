<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDynamicInitialConditionError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsDynamicInitialConditionError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsDynamicInitialConditionError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Errors for dynamic initial conditions

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsDynamicInitialConditionError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsDynamicInitialConditionError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsDynamicInitialConditionError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsDynamicInitialConditionError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsDynamicInitialConditionError\_AllValuesZero** | 13 = Values are zeros |
| **swsDynamicInitialConditionError\_CheckAtleastOneComp** | 12 = Select at least one component for the inital condition |
| **swsDynamicInitialConditionError\_CheckOnlyThirdComp** | 14 = Select only the third direction for a reference edge, and specify a non-zero third value |
| **swsDynamicInitialConditionError\_InvalidEntityArray** | 2 = Unable to read data in the entity array, or the entity array is NULL |
| **swsDynamicInitialConditionError\_InvalidRefGeom** | 7 = The reference geometry is NULL |
| **swsDynamicInitialConditionError\_InvalidType** | 11 = The dynamic initial condition type must be specified using an option from [swsDynamicInitialConditionType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDynamicInitialConditionType_e.html) |
| **swsDynamicInitialConditionError\_NoError** | 0 = Successful |
| **swsDynamicInitialConditionError\_NoFacesOnBeamsAllowed** | 5 = Do not select faces on beams |
| **swsDynamicInitialConditionError\_NotAvailable** | 1 = Dynamic initial condition is not available for this study type |
| **swsDynamicInitialConditionError\_OnlyEdgePlaneOrFaceForReference** | 9 = Select only an edge, plane, or face for the reference entity |
| **swsDynamicInitialConditionError\_OnlyFlatFaceOrStraightEdge** | 10 = Select only a flat face, straight edge, or plane as the reference entity |
| **swsDynamicInitialConditionError\_RefGeomAlreadySelected** | 8 = The reference geometry is already selected |
| **swsDynamicInitialConditionError\_SelectOnlyBeams** | 4 = Select only beam bodies |
| **swsDynamicInitialConditionError\_SelectOnlyFaceBodyOrComps** | 6 = Select only faces, bodies, or components |
| **swsDynamicInitialConditionError\_SelectOnlyJoints** | 3 = Select only joints |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)