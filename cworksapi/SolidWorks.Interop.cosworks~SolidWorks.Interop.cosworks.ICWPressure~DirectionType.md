<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~DirectionType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DirectionType Property (ICWPressure) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html) : DirectionType Property (ICWPressure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets how this pressure is applied along the specified reference geometry.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DirectionType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPressure Dim value As System.Integer   instance.DirectionType = value   value = instance.DirectionType ``` | |

| C# |  |
| --- | --- |
| ``` System.int DirectionType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DirectionType {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Pressure direction type (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPressure::DirectionType.

# ![](dotnetimages/collapse.gif)Requirements

This property is valid only if [ICWPressure::PressureType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PressureType.html) is [swsPressureType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureType_e.html).swsPressureTypeUseReferenceGeometry.

Pressure direction type depends on the reference geometry that is set using [ICWPressure::SetReferenceGeometry](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetReferenceGeometry.html).

| If direction reference is... | Then set this property to a direction as defined in... |
| --- | --- |
| Planar face or reference plane | [swsPressureReferenceGeometryPlanarType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureReferenceGeometryPlanarType_e.html) |
| Cylindrical face | [swsPressureReferenceGeometryCylindricalType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureReferenceGeometryCylindricalType_e.html) |
| Reference axis | [swsPressureReferenceGeometryReferenceAxisType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureReferenceGeometryReferenceAxisType_e.html) |
| Edge | [swsPressureReferenceGeometryEdgeType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureReferenceGeometryEdgeType_e.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[ICWPressure Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0