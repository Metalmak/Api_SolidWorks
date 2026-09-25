<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAutodimStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAutodimStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Statuses returned by ISketch::AutoDimension2 and IDrawingDoc::AutoDimension.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAutodimStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAutodimStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAutodimStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAutodimStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAutodimStatus3DSketchNotSupported** | 5 = Cannot autodimension a 3D sketch |
| **swAutodimStatusAlgorithmFailed** | 17 = Unspecified algorithm failure |
| **swAutodimStatusBadOptionValue** | 1 = An option value for an argument is out of range |
| **swAutodimStatusCenterlineNotAllowed** | 10 = The centerline scheme is not valid for sketches that cannot be revolved to create valid features |
| **swAutodimStatusDatumLineNotCenterline** | 14 = The datum must be a centerline for the centerline scheme |
| **swAutodimStatusDatumLineNotHorizontal** | 16 = If the sketch line is a datum, it must be horizontal for horizontal dimensions |
| **swAutodimStatusDatumLineNotVertical** | 15 = If the sketch line is a datum, it must be vertical for vertical dimension |
| **swAutodimStatusDatumNotSupplied** | 11 = No datum was selected for either the horizontal or vertical dimensioning schemes |
| **swAutodimStatusDatumNotUnique** | 12 = More than one datum was selected for either the horizontal or vertical dimensioning schemes |
| **swAutodimStatusDatumNotValidType** | 13 = One of the selected datums is not valid. Valid types are sketch points and sketch lines |
| **swAutodimStatusDocTypeNotSupported** | 3 = Only part and assemblies documents are supported |
| **swAutodimStatusEntitiesNotValid** | 9 = The entitiesToDimension argument has the value of [swAutodimEntitiesSelected](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimEntities_e.html), but the marked entities are not valid |
| **swAutodimStatusNoActiveDoc** | 2 = No active document |
| **swAutodimStatusNoActiveSketch** | 4 = Can only autodimension an active sketch |
| **swAutodimStatusNoEntities** | 8 = The entitiesToDimension argument has the value of [swAutodimEntitiesSelected](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimEntities_e.html), but no entities were selected and marked with the value [swAutodimMarkEntities](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimMark_e.html) |
| **swAutodimStatusSketchIsEmpty** | 6 = Cannot autodimension an empty sketch |
| **swAutodimStatusSketchIsOverDefined** | 7 = Cannot autodimension an over defined sketch |
| **swAutodimStatusSketchNoSolutionFound** | 18 = Cannot autodimension a sketch for which there is no solution |
| **swAutodimStatusSuccess** | 0 = Sketch successfully dimensioned |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)