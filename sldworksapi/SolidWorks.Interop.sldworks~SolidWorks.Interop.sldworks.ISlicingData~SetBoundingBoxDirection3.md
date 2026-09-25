<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~SetBoundingBoxDirection3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBoundingBoxDirection3 Method (ISlicingData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISlicingData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html) : SetBoundingBoxDirection3 Method (ISlicingData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Direction*
:   For linear slicing:

        -500.0 < left manipulator < 0.0

    For radial slicing:

        0.0 < inner radius < outer radius

    (see **Remarks**)

Sets bounding box direction 3 (left manipulator for linear slicing, inner radius for radial slicing).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBoundingBoxDirection3( _    ByVal Direction As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISlicingData Dim Direction As System.Double Dim value As System.Boolean   value = instance.SetBoundingBoxDirection3(Direction) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBoundingBoxDirection3(     System.double Direction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBoundingBoxDirection3(  &   System.double Direction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   For linear slicing:

        -500.0 < left manipulator < 0.0

    For radial slicing:

        0.0 < inner radius < outer radius

    (see **Remarks**)

#### Return Value

True if direction 3 of bounding box successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SlicingData::SetBoundingBoxDirection3.

# ![](dotnetimages/collapse.gif)Example

See the [ISlicingData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Use these methods to adjust the slicing volume to include or exclude geometry for slicing:

* [ISlicingData::SetBoundingBoxDirection1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~SetBoundingBoxDirection1.html)* [ISlicingData::SetBoundingBoxDirection2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~SetBoundingBoxDirection2.html)* ISlicingData::SetBoundingBoxDirection3* [ISlicingData::SetBoundingBoxDirection4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~SetBoundingBoxDirection4.html)

This method fails when:

* Direction exceeds the specified limits.* The bounding box cannot be created because [ISlicingData::PlaneReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~PlaneReferences.html) has not been set.

# ![](dotnetimages/collapse.gif)See Also

####

[ISlicingData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html)

[ISlicingData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData_members.html)

[ISlicingData::GetBoundingBoxDirection3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~GetBoundingBoxDirection3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0