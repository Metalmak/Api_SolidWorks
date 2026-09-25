<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRestraintType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRestraintType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRestraintType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Restraint types

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRestraintType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRestraintType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRestraintType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRestraintType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRestraintTypeCyclicSymmetry** | 9 = Cyclic symmetry |
| **swsRestraintTypeCylindricalFaces** | 7 = On cylindrical faces; specify translations for solids or translations and rotations for shells and beams |
| **swsRestraintTypeFixed** | 0 = Fixed (set translations and rotations to zero) |
| **swsRestraintTypeFlatFace** | 6 = On flat face; specify translations for solids or translations and rotations for shells and beams |
| **swsRestraintTypeHinge** | 4 = Hinge |
| **swsRestraintTypeImmovable** | 1 = Immovable (set translations to zero) |
| **swsRestraintTypeReferenceGeometry** | 5 = Use reference geometry |
| **swsRestraintTypeRoller** | 3 = Roller |
| **swsRestraintTypeSphericalSurface** | 8 = On spherical faces; specify translations for solids or translations and rotations for shells and beams |
| **swsRestraintTypeSymmetric** | 2 = Symmetric |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)