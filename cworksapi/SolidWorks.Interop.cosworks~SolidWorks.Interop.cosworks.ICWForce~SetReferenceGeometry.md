<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetReferenceGeometry.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReferenceGeometry Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : SetReferenceGeometry Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RefEntity*
:   Reference direction entity (see **Remarks**)

Sets the reference entity along whose direction this force is applied.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReferenceGeometry( _    ByVal RefEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim RefEntity As System.Object   instance.SetReferenceGeometry(RefEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReferenceGeometry(     System.object RefEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReferenceGeometry(  &   System.Object^ RefEntity ) ``` | |

#### Parameters

*RefEntity*
:   Reference direction entity (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::SetReferenceGeometry.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWForce::ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) is set to [swsForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceType_e.html).swsForceTypeForceOrMoment or swsForceType\_e.swsForceTypeTorque.

For forces or moments, specify RefEntity with a face, plane, or edge. For torques, specify RefEntity with a cylindrical face or axis.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::NormalForceOrTorqueValue Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~NormalForceOrTorqueValue.html)

[ICWForce::Unit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Unit.html)

[ICWForce::GetForceComponentValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetForceComponentValues.html)

[ICWForce::GetMomentComponentValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues.html)

[ICWForce::InsertEntity Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~InsertEntity.html)

[ICWForce::SetForceComponentValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues.html)

[ICWForce::SetMomentComponentValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0