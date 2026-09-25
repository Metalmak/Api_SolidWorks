<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~GetBodyOutline.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBodyOutline Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : GetBodyOutline Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyVar*
:   Array of bodies

*Direction*
:   Direction of view

*Tolerance*
:   Tolerance (Parasolid default 0.00001)

*CurvesOut*
:   Array of 3D trimmed curves that form the outline

*TopolEntities*
:   Array of topological entities associated with the outline

*Outline*
:   Array of integers indicating which curves belong to which outline

Obsolete. Superseded by [IModeler::GetBodyOutline2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~GetBodyOutline2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBodyOutline( _    ByVal BodyVar As System.Object, _    ByVal Direction As MathVector, _    ByVal Tolerance As System.Double, _    ByRef CurvesOut As System.Object, _    ByRef TopolEntities As System.Object, _    ByRef Outline As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim BodyVar As System.Object Dim Direction As MathVector Dim Tolerance As System.Double Dim CurvesOut As System.Object Dim TopolEntities As System.Object Dim Outline As System.Object Dim value As System.Integer   value = instance.GetBodyOutline(BodyVar, Direction, Tolerance, CurvesOut, TopolEntities, Outline) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetBodyOutline(     System.object BodyVar,    MathVector Direction,    System.double Tolerance,    out System.object CurvesOut,    out System.object TopolEntities,    out System.object Outline ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetBodyOutline(  &   System.Object^ BodyVar, &   MathVector^ Direction, &   System.double Tolerance, &   [Out] System.Object^ CurvesOut, &   [Out] System.Object^ TopolEntities, &   [Out] System.Object^ Outline ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodyVar*
:   Array of bodies

*Direction*
:   Direction of view

*Tolerance*
:   Tolerance (Parasolid default 0.00001)

*CurvesOut*
:   Array of 3D trimmed curves that form the outline

*TopolEntities*
:   Array of topological entities associated with the outline

*Outline*
:   Array of integers indicating which curves belong to which outline

#### Return Value

Number of curves that form the outline of a body

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::GetBodyOutline.

# ![](dotnetimages/collapse.gif)Remarks

See Parasolid's documentation of PK\_BODY\_make\_curves\_outline for more information about the output.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0