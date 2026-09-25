<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~GetAutoFilletCorners.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAutoFilletCorners Method (IExtrudeFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) : GetAutoFilletCorners Method (IExtrudeFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the corners of this thin feature are automatically filleted.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAutoFilletCorners() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExtrudeFeatureData2 Dim value As System.Boolean   value = instance.GetAutoFilletCorners() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetAutoFilletCorners() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetAutoFilletCorners(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the corners are automatically filleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExtrudeFeatureData2::GetAutoFilletCorners.

# ![](dotnetimages/collapse.gif)Remarks

This method only applies to thin feature extrusions. If the feature is not a thin feature extrusion, then the return value is false, and the COM version of this method returns S\_false in the status return value.

To get the fillet radius, use [IExtrudeFeatureData2::GetAutoFilletRadius](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExtrudeFeatureData2~GetAutoFilletRadius.html). To set automatic fillets and radius, use [IExtrudeFeatureData2::SetAutoFillet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExtrudeFeatureData2~SetAutoFillet.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html)

[IExtrudeFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2_members.html)

[IExtrudeFeatureData2::IsThinFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~IsThinFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP5, Revision Number 12.5