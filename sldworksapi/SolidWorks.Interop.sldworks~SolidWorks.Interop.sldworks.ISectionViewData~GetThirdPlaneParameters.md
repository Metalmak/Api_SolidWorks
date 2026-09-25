<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetThirdPlaneParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetThirdPlaneParameters Method (ISectionViewData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html) : GetThirdPlaneParameters Method (ISectionViewData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PlaneCenter*
:   [Plane center point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html)

*PlaneVector*
:   [Plane normal vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html)

Gets the third transformed plane's parameters for this section view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetThirdPlaneParameters( _    ByRef PlaneCenter As MathPoint, _    ByRef PlaneVector As MathVector _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISectionViewData Dim PlaneCenter As MathPoint Dim PlaneVector As MathVector   instance.GetThirdPlaneParameters(PlaneCenter, PlaneVector) ``` | |

| C# |  |
| --- | --- |
| ``` void GetThirdPlaneParameters(     out MathPoint PlaneCenter,    out MathVector PlaneVector ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetThirdPlaneParameters(  &   [Out] MathPoint^ PlaneCenter, &   [Out] MathVector^ PlaneVector ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PlaneCenter*
:   [Plane center point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html)

*PlaneVector*
:   [Plane normal vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SectionViewData::GetThirdPlaneParameters.

# ![](dotnetimages/collapse.gif)See Also

####

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)

[ISectionViewData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData_members.html)

[ISectionViewData::GetFirstPlaneParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetFirstPlaneParameters.html)

[ISectionViewData::GetSecondPlaneParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetSecondPlaneParameters.html)

[ISectionViewData::FirstPlane Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~FirstPlane.html)

[ISectionViewData::SecondPlane Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~SecondPlane.html)

[ISectionViewData::ThirdPlane Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~ThirdPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0