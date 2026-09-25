<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateEllipse.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipse Method (IModeler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CreateEllipse Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   Array of 3 doubles describing the center of the ellipse

*MajorRadius*
:   Major radius of ellipse

*MinorRadius*
:   Minor radius of ellipse

*MajorAxis*
:   Array of 3 doubles describing the major axis of the ellipse

*MinorAxis*
:   Array of 3 doubles describing the minor axis of the ellipse

Creates a temporary elliptical curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipse( _    ByVal Center As System.Object, _    ByVal MajorRadius As System.Double, _    ByVal MinorRadius As System.Double, _    ByVal MajorAxis As System.Object, _    ByVal MinorAxis As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Center As System.Object Dim MajorRadius As System.Double Dim MinorRadius As System.Double Dim MajorAxis As System.Object Dim MinorAxis As System.Object Dim value As System.Object   value = instance.CreateEllipse(Center, MajorRadius, MinorRadius, MajorAxis, MinorAxis) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateEllipse(     System.object Center,    System.double MajorRadius,    System.double MinorRadius,    System.object MajorAxis,    System.object MinorAxis ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateEllipse(  &   System.Object^ Center, &   System.double MajorRadius, &   System.double MinorRadius, &   System.Object^ MajorAxis, &   System.Object^ MinorAxis ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   Array of 3 doubles describing the center of the ellipse

*MajorRadius*
:   Major radius of ellipse

*MinorRadius*
:   Minor radius of ellipse

*MajorAxis*
:   Array of 3 doubles describing the major axis of the ellipse

*MinorAxis*
:   Array of 3 doubles describing the minor axis of the ellipse

#### Return Value

[Curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CreateEllipse.

# ![](dotnetimages/collapse.gif)Example

[Create Temporary Elliptical Extrusion (VBA)](Create_Temporary_Elliptical_Extrusion_Example_VB.htm)

[Create Temporary Elliptical Extrusion (VB.NET)](Create_Temporary_Elliptical_Extrusion_VBNET.htm)

[Create Temporary Elliptical Extrusion (C#)](Create_Temporary_Elliptical_Extrusion_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::CreateArc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateArc.html)

[IModeler::ICreateArc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateArc.html)

[IModeler::CreateLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateLine.html)

[IModeler::ICreateLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateLine.html)

[IModeler::ICreateEllipse Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateEllipse.html)

[IModeler::CreateExtrudedBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateExtrudedBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP01, Revision Number 20.1