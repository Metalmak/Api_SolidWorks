<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetLocationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetLocationValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : GetLocationValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DXValue*
:   X-coordinate

*DYValue*
:   Y-coordinate

*DZValue*
:   Z-coordinate

Gets the coordinates of the point of application of this remote load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetLocationValues( _    ByRef DXValue As System.Double, _    ByRef DYValue As System.Double, _    ByRef DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim DXValue As System.Double Dim DYValue As System.Double Dim DZValue As System.Double   instance.GetLocationValues(DXValue, DYValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void GetLocationValues(     out System.double DXValue,    out System.double DYValue,    out System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetLocationValues(  &   [Out] System.double DXValue, &   [Out] System.double DYValue, &   [Out] System.double DZValue ) ``` | |

#### Parameters

*DXValue*
:   X-coordinate

*DYValue*
:   Y-coordinate

*DZValue*
:   Z-coordinate

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::GetLocationValues.

# ![](dotnetimages/collapse.gif)Example

[Add Remote Load (C#)](Add_Remote_Load_Example_CSharp.htm)

[Add Remote Load (VB.NET)](Add_Remote_Load_Example_VBNET.htm)

[Add Remote Load (VBA)](Add_Remote_Load_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::SetLocationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetLocationValues.html)

[ICWRemoteLoad::LocationUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~LocationUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0