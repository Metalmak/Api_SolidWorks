<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop~RevolvePlanarLoop.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RevolvePlanarLoop Method (ILoop) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILoop Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop.html) : RevolvePlanarLoop Method (ILoop) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*

*Y*

*Z*

*Axisx*

*Axisy*

*Axisz*

*RevAngle*

Obsolete. Superseded by [ILoop2::RevolvePlanarLoop](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ILoop2~RevolvePlanarLoop.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RevolvePlanarLoop( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal Axisx As System.Double, _    ByVal Axisy As System.Double, _    ByVal Axisz As System.Double, _    ByVal RevAngle As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILoop Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim Axisx As System.Double Dim Axisy As System.Double Dim Axisz As System.Double Dim RevAngle As System.Double Dim value As System.Object   value = instance.RevolvePlanarLoop(X, Y, Z, Axisx, Axisy, Axisz, RevAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.object RevolvePlanarLoop(     System.double X,    System.double Y,    System.double Z,    System.double Axisx,    System.double Axisy,    System.double Axisz,    System.double RevAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ RevolvePlanarLoop(  &   System.double X, &   System.double Y, &   System.double Z, &   System.double Axisx, &   System.double Axisy, &   System.double Axisz, &   System.double RevAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*

*Y*

*Z*

*Axisx*

*Axisy*

*Axisz*

*RevAngle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Loop::RevolvePlanarLoop.

# ![](dotnetimages/collapse.gif)See Also

####

[ILoop Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop.html)

[ILoop Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop_members.html)