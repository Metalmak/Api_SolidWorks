<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ThickenSheet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ThickenSheet Method (IModeler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ThickenSheet Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sheet*
:   Sheet body that defines the profile for the temporary thickened [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Thickness*
:   Thickness of the temporary thickened body

*Direction*
:   Direction in which to thicken the sheet body as defined in swThickenDirection\_e

Thickens a sheet body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ThickenSheet( _    ByVal Sheet As Body2, _    ByVal Thickness As System.Double, _    ByVal Direction As System.Integer _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Sheet As Body2 Dim Thickness As System.Double Dim Direction As System.Integer Dim value As Body2   value = instance.ThickenSheet(Sheet, Thickness, Direction) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 ThickenSheet(     Body2 Sheet,    System.double Thickness,    System.int Direction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ ThickenSheet(  &   Body2^ Sheet, &   System.double Thickness, &   System.int Direction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*
:   Sheet body that defines the profile for the temporary thickened [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Thickness*
:   Thickness of the temporary thickened body

*Direction*
:   Direction in which to thicken the sheet body as defined in swThickenDirection\_e

#### Return Value

Temporary thickened [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ThickenSheet.

# ![](dotnetimages/collapse.gif)Example

[Thicken Sheet Body (VBA)](Thicken_Sheet_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you set Direction to swThickenDirection\_Both, then the value set for Thickness is used in both directions.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0