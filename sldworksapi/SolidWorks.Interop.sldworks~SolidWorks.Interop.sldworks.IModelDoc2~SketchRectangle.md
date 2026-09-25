<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchRectangle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchRectangle Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchRectangle Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Val1*
:   Upper-left x value in meters

*Val2*
:   Upper-left y value in meters

*Z1*
:   Upper-left z value in meters

*Val3*
:   Lower-right x value in meters

*Val4*
:   Lower-right y value in meters

*Z2*
:   Lower-right z value in meters

*Val5*
:   Not used

Obsolete. Superseded by [ISketchManager::CreateCornerRectangle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateCornerRectangle.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchRectangle( _    ByVal Val1 As System.Double, _    ByVal Val2 As System.Double, _    ByVal Z1 As System.Double, _    ByVal Val3 As System.Double, _    ByVal Val4 As System.Double, _    ByVal Z2 As System.Double, _    ByVal Val5 As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Val1 As System.Double Dim Val2 As System.Double Dim Z1 As System.Double Dim Val3 As System.Double Dim Val4 As System.Double Dim Z2 As System.Double Dim Val5 As System.Boolean   instance.SketchRectangle(Val1, Val2, Z1, Val3, Val4, Z2, Val5) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchRectangle(     System.double Val1,    System.double Val2,    System.double Z1,    System.double Val3,    System.double Val4,    System.double Z2,    System.bool Val5 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchRectangle(  &   System.double Val1, &   System.double Val2, &   System.double Z1, &   System.double Val3, &   System.double Val4, &   System.double Z2, &   System.bool Val5 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Val1*
:   Upper-left x value in meters

*Val2*
:   Upper-left y value in meters

*Z1*
:   Upper-left z value in meters

*Val3*
:   Lower-right x value in meters

*Val4*
:   Lower-right y value in meters

*Z2*
:   Lower-right z value in meters

*Val5*
:   Not used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchRectangle.

# ![](dotnetimages/collapse.gif)Example

[Create Revolve Features (VBA)](Create_Revolve_Features_Example_VB.htm)

[Connect to SOLIDWORKS Session (C#)](Connect_to_SOLIDWORKS_Session_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::SketchRectangleAtAnyAngle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchRectangleAtAnyAngle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0