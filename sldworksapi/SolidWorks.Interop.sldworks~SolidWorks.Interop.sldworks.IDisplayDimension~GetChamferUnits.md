<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetChamferUnits.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetChamferUnits Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : GetChamferUnits Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LengthUnit*
:   Unit of length as defined in swLengthUnit\_e

*AngularUnit*
:   Unit of angle as defined in swAngleUnit\_e

Gets the local units of measurement for a chamfer display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetChamferUnits( _    ByRef LengthUnit As System.Integer, _    ByRef AngularUnit As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim LengthUnit As System.Integer Dim AngularUnit As System.Integer Dim value As System.Boolean   value = instance.GetChamferUnits(LengthUnit, AngularUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetChamferUnits(     out System.int LengthUnit,    out System.int AngularUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetChamferUnits(  &   [Out] System.int LengthUnit, &   [Out] System.int AngularUnit ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LengthUnit*
:   Unit of length as defined in swLengthUnit\_e

*AngularUnit*
:   Unit of angle as defined in swAngleUnit\_e

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::GetChamferUnits.

# ![](dotnetimages/collapse.gif)Example

[Get Chamfer Display Dimension (C#)](Get_Chamfer_Display_Dimension_Example_CSharp.htm)

[Get Chamfer Display Dimension (VB.NET)](Get_Chamfer_Display_Dimension_Example_VBNET.htm)

[Get Chamfer Display Dimension (VBA)](Get_Chamfer_Display_Dimension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The unit display setting of a chamfer display dimension is controlled by a value stored in one of two places: on the owning document or on the individual display dimension. Use [IDisplayDimension::GetUseDocUnits](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetUseDocUnits.html) to determine whether the units settings are local or from the owning document. If IDisplayDimension::GetUseDocUnits returns true, then the units settings are from the owning document, and this API returns -1 for both length and angle units of measurement.

Local unit information for a chamfer display dimension is in force when Override Units is selected on the Other tab of the dimension's PropertyManager page. If Override Units is selected, then this API returns units as defined in swLengthUnit\_e (length measurement) and swAngleUnit\_e (angle measurement).

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::GetUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetUnits.html)

[IDisplayDimension::ChamferPrecision Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~ChamferPrecision.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0