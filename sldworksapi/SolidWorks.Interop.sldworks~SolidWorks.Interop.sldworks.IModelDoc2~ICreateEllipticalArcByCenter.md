<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArcByCenter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateEllipticalArcByCenter Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ICreateEllipticalArcByCenter Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the ellipse center

*Major*
:   :   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the major axis

*Minor*
:   :   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the minor axis

*Start*
:   :   Array of 3 doubles (x1, y1, z1) in meters that describe the start point of the ellipse

*End*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the end point of the ellipse

Creates an elliptical arc trimmed between two points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ICreateEllipticalArcByCenter( _    ByRef Center As System.Double, _    ByRef Major As System.Double, _    ByRef Minor As System.Double, _    ByRef Start As System.Double, _    ByRef End As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Center As System.Double Dim Major As System.Double Dim Minor As System.Double Dim Start As System.Double Dim End As System.Double   instance.ICreateEllipticalArcByCenter(Center, Major, Minor, Start, End) ``` | |

| C# |  |
| --- | --- |
| ``` void ICreateEllipticalArcByCenter(     ref System.double Center,    ref System.double Major,    ref System.double Minor,    ref System.double Start,    ref System.double End ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ICreateEllipticalArcByCenter(  &   System.double% Center, &   System.double% Major, &   System.double% Minor, &   System.double% Start, &   System.double% End ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   Array of 3 doubles (x1, y1, z1) in meters that describe the ellipse center

*Major*
:   :   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the major axis

    *Minor*
    :   :   Array of 3 doubles (x1, y1, z1) in meters that describe a point on the ellipse and on the minor axis

        *Start*
        :   :   Array of 3 doubles (x1, y1, z1) in meters that describe the start point of the ellipse

            *End*
            :   Array of 3 doubles (x1, y1, z1) in meters that describe the end point of the ellipse

#### Return Value

True if successfully created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ICreateEllipticalArcByCenter.

# ![](dotnetimages/collapse.gif)Remarks

The Start and End arguments should be specified in a counter-clockwise (CCW) manner.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::CreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipse2.html)

[IModelDoc2::CreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArc2.html)

[IModelDoc2::CreateEllipticalArcByCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenter.html)

[IModelDoc2::CreateEllipticalArcByCenterVB Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipticalArcByCenterVB.html)

[IModelDoc2::ICreateEllipse2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipse2.html)

[IModelDoc2::ICreateEllipticalArc2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ICreateEllipticalArc2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0