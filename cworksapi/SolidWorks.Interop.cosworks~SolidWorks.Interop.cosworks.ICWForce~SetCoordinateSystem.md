<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetCoordinateSystem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetCoordinateSystem Method (ICWForce) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : SetCoordinateSystem Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispCoordinateSystem*
:   Coordinate system

Sets the coordinate system used for defining a force of nonuniform distribution.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetCoordinateSystem( _    ByVal DispCoordinateSystem As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim DispCoordinateSystem As System.Object   instance.SetCoordinateSystem(DispCoordinateSystem) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCoordinateSystem(     System.object DispCoordinateSystem ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCoordinateSystem(  &   System.Object^ DispCoordinateSystem ) ``` | |

#### Parameters

*DispCoordinateSystem*
:   Coordinate system

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::SetCoordinateSystem.

# ![](dotnetimages/collapse.gif)Example

[Add Nonuniform Force Distribution (VBA)](Add_Force_Example_VB.htm)

[Add Nonuniform Force Distribution (VB.NET)](Add_Force_Example_VBNET.htm)

[Add Nonuniform Force Distribution (C#)](Add_Force_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWForce::IncludeNonUniformDistribution2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~IncludeNonUniformDistribution2.html) is set to -1 or true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::GetCoordinateSystem Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetCoordinateSystem.html)

[ICWForce::Equation Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~Equation.html)

[ICWForce::EquationAngularUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationAngularUnit.html)

[ICWForce::EquationCoordinateSystemType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationCoordinateSystemType.html)

[ICWForce::EquationLinearUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~EquationLinearUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0