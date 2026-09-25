<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetMiddleSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetMiddleSurface Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IGetMiddleSurface Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PlacementPercentage*
:   Position where to insert the midsurface in the body; value of 50 indicates to insert the surface in the middle

*Face1List*
:   Array of faces into which the midsurface will be or was inserted; you can provide an array of faces for this parameter and Face2List; if you do not, then the faces are determined internally

*Face2List*
:   Array of faces into which the midsurface will be or was inserted; you can provide an array of faces for this parameter and Face1List; if you do not, then the faces are determined internally

*Thickness*
:   Array containing minimum and maximum thickness of sheet metal for pairs of faces

*MiddleSurfaceBody*
:   [Middle surface body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

Inserts a midsurface in a body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetMiddleSurface( _    ByVal PlacementPercentage As System.Double, _    ByRef Face1List As System.Object, _    ByRef Face2List As System.Object, _    ByRef Thickness As System.Object, _    ByRef MiddleSurfaceBody As Body2 _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim PlacementPercentage As System.Double Dim Face1List As System.Object Dim Face2List As System.Object Dim Thickness As System.Object Dim MiddleSurfaceBody As Body2 Dim value As System.Integer   value = instance.IGetMiddleSurface(PlacementPercentage, Face1List, Face2List, Thickness, MiddleSurfaceBody) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetMiddleSurface(     System.double PlacementPercentage,    out System.object Face1List,    out System.object Face2List,    out System.object Thickness,    out Body2 MiddleSurfaceBody ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetMiddleSurface(  &   System.double PlacementPercentage, &   [Out] System.Object^ Face1List, &   [Out] System.Object^ Face2List, &   [Out] System.Object^ Thickness, &   [Out] Body2^ MiddleSurfaceBody ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PlacementPercentage*
:   Position where to insert the midsurface in the body; value of 50 indicates to insert the surface in the middle

*Face1List*
:   Array of faces into which the midsurface will be or was inserted; you can provide an array of faces for this parameter and Face2List; if you do not, then the faces are determined internally

*Face2List*
:   Array of faces into which the midsurface will be or was inserted; you can provide an array of faces for this parameter and Face1List; if you do not, then the faces are determined internally

*Thickness*
:   Array containing minimum and maximum thickness of sheet metal for pairs of faces

*MiddleSurfaceBody*
:   [Middle surface body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

#### Return Value

0 if no errors; -1 if errors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IGetMiddleSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::GetMiddleSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMiddleSurface.html)