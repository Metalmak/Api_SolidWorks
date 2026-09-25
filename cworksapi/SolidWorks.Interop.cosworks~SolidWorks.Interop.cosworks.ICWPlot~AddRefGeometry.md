<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot~AddRefGeometry.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddRefGeometry Method (ICWPlot) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html) : AddRefGeometry Method (ICWPlot) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NDispType*
:   Type of reference geometry as defined in [swsRefDispType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRefDispType_e.html)

*DispPlaneAxisCoordSys*
:   Plane, axis, or coordinate system

Specifies the reference geometry for directional component plots.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddRefGeometry( _    ByVal NDispType As System.Integer, _    ByVal DispPlaneAxisCoordSys As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPlot Dim NDispType As System.Integer Dim DispPlaneAxisCoordSys As System.Object Dim value As System.Integer   value = instance.AddRefGeometry(NDispType, DispPlaneAxisCoordSys) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddRefGeometry(     System.int NDispType,    System.object DispPlaneAxisCoordSys ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddRefGeometry(  &   System.int NDispType, &   System.Object^ DispPlaneAxisCoordSys ) ``` | |

#### Parameters

*NDispType*
:   Type of reference geometry as defined in [swsRefDispType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRefDispType_e.html)

*DispPlaneAxisCoordSys*
:   Plane, axis, or coordinate system

#### Return Value

Error code as defined in [swsResultPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPlot::AddRefGeometry.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for the following directional component plots:

* Displacement* Mode Shape/Amplitude* Strain* Stress* Thermal

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPlot Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot.html)

[ICWPlot Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPlot_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0