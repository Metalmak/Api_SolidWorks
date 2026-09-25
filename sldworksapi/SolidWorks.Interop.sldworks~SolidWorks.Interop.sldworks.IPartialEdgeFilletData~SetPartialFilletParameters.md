<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~SetPartialFilletParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPartialFilletParameters Method (IPartialEdgeFilletData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartialEdgeFilletData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData.html) : SetPartialFilletParameters Method (IPartialEdgeFilletData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AlongEdgeDirection*
:   True to start the fillet at the start point of the edge, false to start the fillet at the end point of the edge

*StartCondition*
:   Start condition as defined in swSimpleFilletPartialEdgeCondition\_e (see **Remarks**)

*StartValue*
:   Distance or percent offset from the start point (see **Remarks**)

*StartReference*
:   Offset reference (2D/3D sketch [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html), reference [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html), planar [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)); valid only if StartCondition is swPartialEdgeReferenceOffset

*EndCondition*
:   End condition as defined in swSimpleFilletPartialEdgeCondition\_e (see **Remarks**)

*EndValue*
:   Distance or percent offset from the end point (see **Remarks**)

*EndReference*
:   Offset reference (2D/3D sketch [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html), reference [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html), planar [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)); valid only if EndCondition is swPartialEdgeReferenceOffset

Sets the properties of this partial edge fillet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPartialFilletParameters( _    ByVal AlongEdgeDirection As System.Boolean, _    ByVal StartCondition As System.Integer, _    ByVal StartValue As System.Double, _    ByVal StartReference As System.Object, _    ByVal EndCondition As System.Integer, _    ByVal EndValue As System.Double, _    ByVal EndReference As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartialEdgeFilletData Dim AlongEdgeDirection As System.Boolean Dim StartCondition As System.Integer Dim StartValue As System.Double Dim StartReference As System.Object Dim EndCondition As System.Integer Dim EndValue As System.Double Dim EndReference As System.Object Dim value As System.Integer   value = instance.SetPartialFilletParameters(AlongEdgeDirection, StartCondition, StartValue, StartReference, EndCondition, EndValue, EndReference) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPartialFilletParameters(     System.bool AlongEdgeDirection,    System.int StartCondition,    System.double StartValue,    System.object StartReference,    System.int EndCondition,    System.double EndValue,    System.object EndReference ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPartialFilletParameters(  &   System.bool AlongEdgeDirection, &   System.int StartCondition, &   System.double StartValue, &   System.Object^ StartReference, &   System.int EndCondition, &   System.double EndValue, &   System.Object^ EndReference ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AlongEdgeDirection*
:   True to start the fillet at the start point of the edge, false to start the fillet at the end point of the edge

*StartCondition*
:   Start condition as defined in swSimpleFilletPartialEdgeCondition\_e (see **Remarks**)

*StartValue*
:   Distance or percent offset from the start point (see **Remarks**)

*StartReference*
:   Offset reference (2D/3D sketch [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html), reference [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html), planar [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)); valid only if StartCondition is swPartialEdgeReferenceOffset

*EndCondition*
:   End condition as defined in swSimpleFilletPartialEdgeCondition\_e (see **Remarks**)

*EndValue*
:   Distance or percent offset from the end point (see **Remarks**)

*EndReference*
:   Offset reference (2D/3D sketch [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html), reference [point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html), planar [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)); valid only if EndCondition is swPartialEdgeReferenceOffset

#### Return Value

Result code as defined in swFeatureError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartialEdgeFilletData::SetPartialFilletParameters.

# ![](dotnetimages/collapse.gif)Example

See the [IPartialEdgeFilletData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

StartValue (or EndValue) is a:

* Distance if StartCondition (or EndCondition) is swSimpleFilletPartialEdgeCondition\_e.swPartialEdgeDistanceOffset.* Percent value if StartCondition (or EndCondition) is swSimpleFilletPartialEdgeCondition\_e.swPartialEdgePercentOffset.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartialEdgeFilletData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData.html)

[IPartialEdgeFilletData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData_members.html)

[IPartialEdgeFilletData::AlongEdgeDirection Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~AlongEdgeDirection.html)

[IPartialEdgeFilletData::DistanceOffsetEnd Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~DistanceOffsetEnd.html)

[IPartialEdgeFilletData::DistanceOffsetStart Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~DistanceOffsetStart.html)

[IPartialEdgeFilletData::PercentOffsetEnd Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~PercentOffsetEnd.html)

[IPartialEdgeFilletData::PercentOffsetStart Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~PercentOffsetStart.html)

[IPartialEdgeFilletData::ReferenceOffsetEnd Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~ReferenceOffsetEnd.html)

[IPartialEdgeFilletData::ReferenceOffsetStart Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData~ReferenceOffsetStart.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0