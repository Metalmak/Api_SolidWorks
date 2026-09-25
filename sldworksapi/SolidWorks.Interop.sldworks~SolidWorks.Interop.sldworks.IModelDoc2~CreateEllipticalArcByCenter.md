<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipticalArcByCenter Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateEllipticalArcByCenter Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   Array of 3 doubles(x1, y1, z1) in meters that describe the ellipse center

*Major*
:   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the major axis

*Minor*
:   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the minor axis

*Start*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the start point of the ellipse

*End*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the end point of the ellipse

Obsolete. Superseded by [SketchManager::CreateEllipticalArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateEllipticalArc.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipticalArcByCenter( _    ByVal Center As System.Object, _    ByVal Major As System.Object, _    ByVal Minor As System.Object, _    ByVal Start As System.Object, _    ByVal End As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Center As System.Object Dim Major As System.Object Dim Minor As System.Object Dim Start As System.Object Dim End As System.Object Dim value As System.Boolean   value = instance.CreateEllipticalArcByCenter(Center, Major, Minor, Start, End) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateEllipticalArcByCenter(     System.object Center,    System.object Major,    System.object Minor,    System.object Start,    System.object End ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateEllipticalArcByCenter(  &   System.Object^ Center, &   System.Object^ Major, &   System.Object^ Minor, &   System.Object^ Start, &   System.Object^ End ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   Array of 3 doubles(x1, y1, z1) in meters that describe the ellipse center

*Major*
:   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the major axis

*Minor*
:   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the minor axis

*Start*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the start point of the ellipse

*End*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the end point of the ellipse

#### Return Value

True if successfully created, false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateEllipticalArcByCenter.

# ![](dotnetimages/collapse.gif)Remarks

The Start and End arguments should be specified in a counter-clockwise (CCW) manner.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::ICreateEllipticalArcByCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArcByCenter.html)

[IModelDoc2::ICreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArc2.html)

[IModelDoc2::ICreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipse2.html)

[IModelDoc2::CreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArc2.html)

[IModelDoc2::CreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipse2.html)

[IModelDoc2::CreateEllipticalArcByCenterVB Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenterVB.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0