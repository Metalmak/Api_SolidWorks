<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~AddVariablePitchHelixFirstPitchAndDiameter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddVariablePitchHelixFirstPitchAndDiameter Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : AddVariablePitchHelixFirstPitchAndDiameter Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstPitch*
:   Pitch, which determines the width of one complete helix turn, measured parallel to the axis of the helix

*FirstDiameter*
:   Diameter, which determines how far the variable-pitch helix segment extends

Adds the first segment to a variable-pitch helix.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddVariablePitchHelixFirstPitchAndDiameter( _    ByVal FirstPitch As System.Double, _    ByVal FirstDiameter As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FirstPitch As System.Double Dim FirstDiameter As System.Double Dim value As System.Boolean   value = instance.AddVariablePitchHelixFirstPitchAndDiameter(FirstPitch, FirstDiameter) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddVariablePitchHelixFirstPitchAndDiameter(     System.double FirstPitch,    System.double FirstDiameter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddVariablePitchHelixFirstPitchAndDiameter(  &   System.double FirstPitch, &   System.double FirstDiameter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstPitch*
:   Pitch, which determines the width of one complete helix turn, measured parallel to the axis of the helix

*FirstDiameter*
:   Diameter, which determines how far the variable-pitch helix segment extends

#### Return Value

True if the first segment of the helix is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::AddVariablePitchHelixPatchAndDiameter.

# ![](dotnetimages/collapse.gif)Example

[Create Variable-pitch Helix (C#)](Create_Variable_Pitch_Helix_Example_CSharp.htm)

[Create Variable-pitch Helix (VB.NET)](Create_Variable_Pitch_Helix_Example_VBNET.htm)

[Create Variable-pitch Helix (VBA)](Create_Variable_Pitch_Helix_Example_VB.htm)

[Create and Modify Variable-pitch Helix (C#)](Create_and_Modify_Variable-pitch_Helix_Example_CSharp.htm)

[Create and Modify Variable-pitch Helix (VB.NET)](Create_and_Modify_Variable-pitch_Helix_Example_VBNET.htm)

[Create and Modify Variable-pitch Helix (VBA)](Create_and_Modify_Variable-pitch_Helix_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create and insert a variable-pitch helix, call:

1. [IFeatureManager::InsertVariablePitchHelix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVariablePitchHelix.html) to create it.- IFeatureManager::AddVariablePitchHelixFirstPitchAndDiamenter to add the first segment.- [IFeatureManager::AddVariablePitchHelixSegment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddVariablePitchHelixSegment.html) one or more times to add the remaining segments.- [IFeatureManager::EndVariablePitchHelix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~EndVariablePitchHelix.html) to insert it.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IHelixFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0