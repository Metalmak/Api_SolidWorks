<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~SetRegionParameterAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetRegionParameterAtIndex Method (IHelixFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHelixFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData.html) : SetRegionParameterAtIndex Method (IHelixFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of the region

*Parameter*
:   Region parameter as defined in swVariablePitchHelixRegionParameter\_e (see **Remarks**)

*PitchValue*
:   Region parameter value

Sets the specified parameter for the specified region in this variable-pitch helix.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetRegionParameterAtIndex( _    ByVal Index As System.Integer, _    ByVal Parameter As System.Integer, _    ByVal PitchValue As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHelixFeatureData Dim Index As System.Integer Dim Parameter As System.Integer Dim PitchValue As System.Double Dim value As System.Integer   value = instance.SetRegionParameterAtIndex(Index, Parameter, PitchValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetRegionParameterAtIndex(     System.int Index,    System.int Parameter,    System.double PitchValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetRegionParameterAtIndex(  &   System.int Index, &   System.int Parameter, &   System.double PitchValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of the region

*Parameter*
:   Region parameter as defined in swVariablePitchHelixRegionParameter\_e (see **Remarks**)

*PitchValue*
:   Region parameter value

#### Return Value

Status of setting region parameters as defined in swSetHelixRegionParameterStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HelixFeatureData::SetRegionParameterAtIndex.

# ![](dotnetimages/collapse.gif)Example

[Create and Modify Variable-pitch Helix (C#)](Create_and_Modify_Variable-pitch_Helix_Example_CSharp.htm)

[Create and Modify Variable-pitch Helix (VB.NET)](Create_and_Modify_Variable-pitch_Helix_Example_VBNET.htm)

[Create and Modify Variable-pitch Helix (VBA)](Create_and_Modify_Variable-pitch_Helix_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If the [helix is defined](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IHelixFeatureData~DefinedBy.html) as...** | **Then you cannot change...** |
| swHelixDefinedBy\_e.swHelixDefinedByHeightAndPitch | Revolution value |
| swHelixDefinedBy\_e.swHelixDefinedByHeightAndRevolution | Pitch value |
| swHelixDefinedBy\_e.swHelixDefinedByPitchAndRevolution | Height value |

|  |  |
| --- | --- |
| **If setting a value for...** | **Then you...** |
| Revolution | Must specify a value greater than the previous region's revolution value and less than the next region's revolution value |
| Pitch for the first region only | Cannot change diameter, height, or revolution |

# ![](dotnetimages/collapse.gif)See Also

####

[IHelixFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData.html)

[IHelixFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData_members.html)

[IHelixFeatureData::VariablePitch Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~VariablePitch.html)

[IHelixFeatureData::PitchCount Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~PitchCount.html)

[IHelixFeatureData::GetRegionParameterAtIndex Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~GetRegionParameterAtIndex.html)

[IHelixFeatureData::InsertRecord Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~InsertRecord.html)

[IHelixFeatureData::DeleteRecord Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~DeleteRecord.html)

[IHelixFeatureData::AddLastRecord Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData~AddLastRecord.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0