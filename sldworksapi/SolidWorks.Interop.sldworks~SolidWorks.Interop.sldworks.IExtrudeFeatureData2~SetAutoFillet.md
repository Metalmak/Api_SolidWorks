<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~SetAutoFillet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAutoFillet Method (IExtrudeFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) : SetAutoFillet Method (IExtrudeFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AutoFillet*
:   True to fillet the corners automatically, false to not

*Radius*
:   Fillet radius, if automatic corner fillets is enabled

Sets the automatic corner fillet properties of this thin feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAutoFillet( _    ByVal AutoFillet As System.Boolean, _    ByVal Radius As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExtrudeFeatureData2 Dim AutoFillet As System.Boolean Dim Radius As System.Double Dim value As System.Boolean   value = instance.SetAutoFillet(AutoFillet, Radius) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetAutoFillet(     System.bool AutoFillet,    System.double Radius ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetAutoFillet(  &   System.bool AutoFillet, &   System.double Radius ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AutoFillet*
:   True to fillet the corners automatically, false to not

*Radius*
:   Fillet radius, if automatic corner fillets is enabled

#### Return Value

True if the corners are automatically filleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExtrudeFeatureData2::SetAutoFillet.

# ![](dotnetimages/collapse.gif)Remarks

This method only applies to thin feature extrusions. If the feature is not a thin feature extrusion, then no action is taken and the COM version of this method returns S\_false in the status return value.

If disabling the automatic corner fillets property (AutoFillet = false), then the Radius value is not used.

To get the automatic corner fillet flag, use [IExtrudeFeatureData2::GetAutoFilletCorners](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExtrudeFeatureData2~GetAutoFilletCorners.html). To get the fillet radius, use [IExtrudeFeatureData2::GetAutoFilletRadius](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExtrudeFeatureData2~GetAutoFilletRadius.html) .

# ![](dotnetimages/collapse.gif)See Also

####

[IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html)

[IExtrudeFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2_members.html)

[IExtrudeFeatureData2::IsThinFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~IsThinFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP5, Revision Number 12.5