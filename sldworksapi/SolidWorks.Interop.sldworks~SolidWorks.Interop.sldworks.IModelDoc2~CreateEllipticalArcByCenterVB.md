<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenterVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipticalArcByCenterVB Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateEllipticalArcByCenterVB Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CenterX*
:   X values for the ellipse center point

*CenterY*
:   Y values for the ellipse center point

*CenterZ*
:   Z values for the ellipse center point

*MajorX*
:   X values for a point on the ellipse and on the major axis

*MajorY*
:   Y values for a point on the ellipse and on the major axis

*MajorZ*
:   Z values for a point on the ellipse and on the major axis

*MinorX*
:   X values for a point on the ellipse and on the minor axis

*MinorY*
:   Y values for a point on the ellipse and on the minor axis

*MinorZ*
:   Z values for a point on the ellipse and on the minor axis

*StartX*
:   X values for CCW elliptical arc start point

*StartY*
:   Y values for CCW elliptical arc start point

*StartZ*
:   Z values for CCW elliptical arc start point

*EndX*
:   X values for CCW elliptical arc end point

*EndY*
:   Y values for CCW elliptical arc end point

*EndZ*
:   Z values for CCW elliptical arc end point

Obsolete. Superseded by [SketchManager::CreateEllipticalArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateEllipticalArc.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipticalArcByCenterVB( _    ByVal CenterX As System.Double, _    ByVal CenterY As System.Double, _    ByVal CenterZ As System.Double, _    ByVal MajorX As System.Double, _    ByVal MajorY As System.Double, _    ByVal MajorZ As System.Double, _    ByVal MinorX As System.Double, _    ByVal MinorY As System.Double, _    ByVal MinorZ As System.Double, _    ByVal StartX As System.Double, _    ByVal StartY As System.Double, _    ByVal StartZ As System.Double, _    ByVal EndX As System.Double, _    ByVal EndY As System.Double, _    ByVal EndZ As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim CenterX As System.Double Dim CenterY As System.Double Dim CenterZ As System.Double Dim MajorX As System.Double Dim MajorY As System.Double Dim MajorZ As System.Double Dim MinorX As System.Double Dim MinorY As System.Double Dim MinorZ As System.Double Dim StartX As System.Double Dim StartY As System.Double Dim StartZ As System.Double Dim EndX As System.Double Dim EndY As System.Double Dim EndZ As System.Double Dim value As System.Boolean   value = instance.CreateEllipticalArcByCenterVB(CenterX, CenterY, CenterZ, MajorX, MajorY, MajorZ, MinorX, MinorY, MinorZ, StartX, StartY, StartZ, EndX, EndY, EndZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateEllipticalArcByCenterVB(     System.double CenterX,    System.double CenterY,    System.double CenterZ,    System.double MajorX,    System.double MajorY,    System.double MajorZ,    System.double MinorX,    System.double MinorY,    System.double MinorZ,    System.double StartX,    System.double StartY,    System.double StartZ,    System.double EndX,    System.double EndY,    System.double EndZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateEllipticalArcByCenterVB(  &   System.double CenterX, &   System.double CenterY, &   System.double CenterZ, &   System.double MajorX, &   System.double MajorY, &   System.double MajorZ, &   System.double MinorX, &   System.double MinorY, &   System.double MinorZ, &   System.double StartX, &   System.double StartY, &   System.double StartZ, &   System.double EndX, &   System.double EndY, &   System.double EndZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CenterX*
:   X values for the ellipse center point

*CenterY*
:   Y values for the ellipse center point

*CenterZ*
:   Z values for the ellipse center point

*MajorX*
:   X values for a point on the ellipse and on the major axis

*MajorY*
:   Y values for a point on the ellipse and on the major axis

*MajorZ*
:   Z values for a point on the ellipse and on the major axis

*MinorX*
:   X values for a point on the ellipse and on the minor axis

*MinorY*
:   Y values for a point on the ellipse and on the minor axis

*MinorZ*
:   Z values for a point on the ellipse and on the minor axis

*StartX*
:   X values for CCW elliptical arc start point

*StartY*
:   Y values for CCW elliptical arc start point

*StartZ*
:   Z values for CCW elliptical arc start point

*EndX*
:   X values for CCW elliptical arc end point

*EndY*
:   Y values for CCW elliptical arc end point

*EndZ*
:   Z values for CCW elliptical arc end point

#### Return Value

True if successfully created, false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateEllipticalArcByCenterVB.

# ![](dotnetimages/collapse.gif)Remarks

The Start\* and End\* arguments should be specified in a counter-clockwise (CCW) manner.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::ICreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipse2.html)

[IModelDoc2::ICreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArc2.html)

[IModelDoc2::ICreateEllipticalArcByCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArcByCenter.html)

[IModelDoc2::CreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipse2.html)

[IModelDoc2::CreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArc2.html)

[IModelDoc2::CreateEllipticalArcByCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0