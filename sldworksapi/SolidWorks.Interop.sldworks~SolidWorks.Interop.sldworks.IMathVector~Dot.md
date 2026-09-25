<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathVector~Dot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Dot Method (IMathVector) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMathVector Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathVector.html) : Dot Method (IMathVector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VectorObjIn*
:   [Math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) to use to determine the dot value

Gets the value of the dot product between two math vectors.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Dot( _    ByVal VectorObjIn As System.Object _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMathVector Dim VectorObjIn As System.Object Dim value As System.Double   value = instance.Dot(VectorObjIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.double Dot(     System.object VectorObjIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double Dot(  &   System.Object^ VectorObjIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VectorObjIn*
:   [Math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) to use to determine the dot value

#### Return Value

Value of the dot product

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MathVector::Dot.

# ![](dotnetimages/collapse.gif)Example

[Get Angle of Hole Not Normal to Face (VBA)](Get_Angle_of_Hole_Not_Normal_to_a_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMathVector Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathVector.html)

[IMathVector Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathVector_members.html)

[IMathVector::IDot Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathVector~IDot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0