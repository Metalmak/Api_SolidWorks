<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateEllipse.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateEllipse Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateEllipse Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the location of the center of the ellipse

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*MajorRadius*
:   Major radius of ellipse

*MinorRadius*
:   Minor radius of ellipse

*MajorAxis*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the major axis of the ellipse

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*MinorAxis*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the minor axis of the ellipse

      * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Creates a temporary elliptical curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateEllipse( _    ByRef Center As System.Double, _    ByVal MajorRadius As System.Double, _    ByVal MinorRadius As System.Double, _    ByRef MajorAxis As System.Double, _    ByRef MinorAxis As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Center As System.Double Dim MajorRadius As System.Double Dim MinorRadius As System.Double Dim MajorAxis As System.Double Dim MinorAxis As System.Double Dim value As Curve   value = instance.ICreateEllipse(Center, MajorRadius, MinorRadius, MajorAxis, MinorAxis) ``` | |

| C# |  |
| --- | --- |
| ``` Curve ICreateEllipse(     ref System.double Center,    System.double MajorRadius,    System.double MinorRadius,    ref System.double MajorAxis,    ref System.double MinorAxis ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ ICreateEllipse(  &   System.double% Center, &   System.double MajorRadius, &   System.double MinorRadius, &   System.double% MajorAxis, &   System.double% MinorAxis ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the location of the center of the ellipse

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*MajorRadius*
:   Major radius of ellipse

*MinorRadius*
:   Minor radius of ellipse

*MajorAxis*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the major axis of the ellipse

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*MinorAxis*
:   * in-process, unmanaged C++: Pointer to an array of 3 doubles describing the minor axis of the ellipse

      * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

[Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::CreateEllipse Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateEllipse.html)

[IModeler::CreateArc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateArc.html)

[IModeler::ICreateArc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateArc.html)

[IModeler::CreateLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateLine.html)

[IModeler::ICreateLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateLine.html)

[IModeler::CreateExtrudedBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateExtrudedBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP01, Revision Number 20.1