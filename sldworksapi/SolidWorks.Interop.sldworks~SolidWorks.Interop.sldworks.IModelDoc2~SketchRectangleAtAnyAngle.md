<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchRectangleAtAnyAngle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchRectangleAtAnyAngle Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchRectangleAtAnyAngle Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Val1*
:   X value of corner 1

*Val2*
:   Y value of corner 1

*Z1*
:   Z value of corner 1

*Val3*
:   X value of corner 2 defining the bottom line from corner 1

*Val4*
:   Y value of corner 2 defining the bottom line from corner 1

*Z2*
:   Z value of corner 2 defining the bottom line from corner 1

*Val3x*
:   X value of corner 3; diagonal to corner 1

*Val3y*
:   Y value of corner 3; diagonal to corner 1

*Z3*
:   Z value of corner 3; diagonal to corner 1

*Val5*
:   True to add automatic constraints to the rectangle geometry, false to not

Obsolete. Superseded by [ISketchManager::Create3PointCornerRectangle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~Create3PointCornerRectangle.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchRectangleAtAnyAngle( _    ByVal Val1 As System.Double, _    ByVal Val2 As System.Double, _    ByVal Z1 As System.Double, _    ByVal Val3 As System.Double, _    ByVal Val4 As System.Double, _    ByVal Z2 As System.Double, _    ByVal Val3x As System.Double, _    ByVal Val3y As System.Double, _    ByVal Z3 As System.Double, _    ByVal Val5 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Val1 As System.Double Dim Val2 As System.Double Dim Z1 As System.Double Dim Val3 As System.Double Dim Val4 As System.Double Dim Z2 As System.Double Dim Val3x As System.Double Dim Val3y As System.Double Dim Z3 As System.Double Dim Val5 As System.Boolean   instance.SketchRectangleAtAnyAngle(Val1, Val2, Z1, Val3, Val4, Z2, Val3x, Val3y, Z3, Val5) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchRectangleAtAnyAngle(     System.double Val1,    System.double Val2,    System.double Z1,    System.double Val3,    System.double Val4,    System.double Z2,    System.double Val3x,    System.double Val3y,    System.double Z3,    System.bool Val5 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchRectangleAtAnyAngle(  &   System.double Val1, &   System.double Val2, &   System.double Z1, &   System.double Val3, &   System.double Val4, &   System.double Z2, &   System.double Val3x, &   System.double Val3y, &   System.double Z3, &   System.bool Val5 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Val1*
:   X value of corner 1

*Val2*
:   Y value of corner 1

*Z1*
:   Z value of corner 1

*Val3*
:   X value of corner 2 defining the bottom line from corner 1

*Val4*
:   Y value of corner 2 defining the bottom line from corner 1

*Z2*
:   Z value of corner 2 defining the bottom line from corner 1

*Val3x*
:   X value of corner 3; diagonal to corner 1

*Val3y*
:   Y value of corner 3; diagonal to corner 1

*Z3*
:   Z value of corner 3; diagonal to corner 1

*Val5*
:   True to add automatic constraints to the rectangle geometry, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchRectangleAtAnyAngle.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::SketchRectangle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchRectangle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0