<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetReferenceGeometry.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReferenceGeometry Method (ICWPressure) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html) : SetReferenceGeometry Method (ICWPressure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RefEntity*
:   Face, edge, plane, or axis

Sets the face, edge, plane, or axis to be used to set the direction of this pressure.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReferenceGeometry( _    ByVal RefEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPressure Dim RefEntity As System.Object   instance.SetReferenceGeometry(RefEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReferenceGeometry(     System.object RefEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReferenceGeometry(  &   System.Object^ RefEntity ) ``` | |

#### Parameters

*RefEntity*
:   Face, edge, plane, or axis

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPressure::SetReferenceGeometry.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWPressure::PressureType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~PressureType.html) is [swsPressureType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPressureType_e.html).swsPressureTypeUseReferenceGeometry.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[ICWPressure Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html)

[ICWPressure::DirectionType Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~DirectionType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0