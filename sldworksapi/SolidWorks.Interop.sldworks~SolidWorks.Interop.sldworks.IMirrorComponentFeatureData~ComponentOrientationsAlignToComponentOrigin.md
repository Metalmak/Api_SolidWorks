<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData~ComponentOrientationsAlignToComponentOrigin.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ComponentOrientationsAlignToComponentOrigin Property (IMirrorComponentFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMirrorComponentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html) : ComponentOrientationsAlignToComponentOrigin Property (IMirrorComponentFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the array of orientations for the components whose axes align to origins.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ComponentOrientationsAlignToComponentOrigin As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMirrorComponentFeatureData Dim value As System.Object   instance.ComponentOrientationsAlignToComponentOrigin = value   value = instance.ComponentOrientationsAlignToComponentOrigin ``` | |

| C# |  |
| --- | --- |
| ``` System.object ComponentOrientationsAlignToComponentOrigin {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ ComponentOrientationsAlignToComponentOrigin {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of swMirrorComponentOrientation2\_e values

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MirrorComponentFeatureData::ComponentOrientationsAlignToComponentOrigin.

# ![](dotnetimages/collapse.gif)Example

See the [IMirrorComponentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

There is a one-to-one mapping between this array and [IMirrorComponentFeatureData::ComponentsToInstanceAlignToComponentOrigin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData~ComponentsToInstanceAlignToComponentOrigin.html). If there are fewer elements in this array than are in IMirrorComponentFeatureData::ComponentsToInstanceAlignToComponentOrigin, then missing orientations default to swMirrorComponentOrientation2\_e.swOrientation\_MirroredX\_MirroredY.

# ![](dotnetimages/collapse.gif)See Also

####

[IMirrorComponentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html)

[IMirrorComponentFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0