<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateFillet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFillet Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateFillet Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Radius*
:   Radius of the fillet in meters

*ConstrainedCorners*
:   Action to take as defined in swConstrainedCornerAction\_e (see **Remarks**)

Creates a sketch fillet using the selected sketch entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFillet( _    ByVal Radius As System.Double, _    ByVal ConstrainedCorners As System.Integer _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Radius As System.Double Dim ConstrainedCorners As System.Integer Dim value As SketchSegment   value = instance.CreateFillet(Radius, ConstrainedCorners) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment CreateFillet(     System.double Radius,    System.int ConstrainedCorners ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ CreateFillet(  &   System.double Radius, &   System.int ConstrainedCorners ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Radius*
:   Radius of the fillet in meters

*ConstrainedCorners*
:   Action to take as defined in swConstrainedCornerAction\_e (see **Remarks**)

#### Return Value

[Sketch segment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) for the fillet

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateFillet.

# ![](dotnetimages/collapse.gif)Example

[Edit Radial Dimension (C#)](Edit_Radial_Dimension_Example_CSharp.htm)

[Edit Radial Dimension (VB.NET)](Edit_Radial_Dimension_Example_VBNET.htm)

[Edit Radial Dimension (VBA)](Edit_Radial_Dimension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The ConstrainedCorners parameter indicates what action to take if the corner to fillet is constrained or dimensioned. If the corner is not constrained or dimensioned, then this parameter is ignored.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0