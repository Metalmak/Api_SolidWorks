<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertVariablePitchHelix.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertVariablePitchHelix Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertVariablePitchHelix Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Reversed*
:   True to reverse the variable-pitch helix, false to not

*Clockwise*
:   True to create the variable-pitch helix in a clockwise direction, false to create in a counter-clockwise direction

*Helixdef*
:   Definition of variable-pitch helix as defined in swHelixDefinedBy\_e; valid enumerators are:

    * swHelixDefinedByPitchAndRevolution

      * swHelixDefinedByHeightandRevolution

        * swHelixDefinedByHeightAndPitch

*Startangle*
:   Angle at which to start the variable-pitch helix

Starts a variable-pitch helix using the selected sketch containing an arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertVariablePitchHelix( _    ByVal Reversed As System.Boolean, _    ByVal Clockwise As System.Boolean, _    ByVal Helixdef As System.Integer, _    ByVal Startangle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Reversed As System.Boolean Dim Clockwise As System.Boolean Dim Helixdef As System.Integer Dim Startangle As System.Double Dim value As System.Boolean   value = instance.InsertVariablePitchHelix(Reversed, Clockwise, Helixdef, Startangle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertVariablePitchHelix(     System.bool Reversed,    System.bool Clockwise,    System.int Helixdef,    System.double Startangle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertVariablePitchHelix(  &   System.bool Reversed, &   System.bool Clockwise, &   System.int Helixdef, &   System.double Startangle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Reversed*
:   True to reverse the variable-pitch helix, false to not

*Clockwise*
:   True to create the variable-pitch helix in a clockwise direction, false to create in a counter-clockwise direction

*Helixdef*
:   Definition of variable-pitch helix as defined in swHelixDefinedBy\_e; valid enumerators are:

    * swHelixDefinedByPitchAndRevolution

      * swHelixDefinedByHeightandRevolution

        * swHelixDefinedByHeightAndPitch

*Startangle*
:   Angle at which to start the variable-pitch helix

#### Return Value

True if the variable-pitch helix is started, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertVariablePitchHelix.

# ![](dotnetimages/collapse.gif)Example

[Create Variable-pitch Helix (C#)](Create_Variable_Pitch_Helix_Example_CSharp.htm)

[Create Variable-pitch Helix (VB.NET)](Create_Variable_Pitch_Helix_Example_VBNET.htm)

[Create Variable-pitch Helix (VBA)](Create_Variable_Pitch_Helix_Example_VB.htm)

[Create and Modify Variable-pitch Helix (C#)](Create_and_Modify_Variable-pitch_Helix_Example_CSharp.htm)

[Create and Modify Variable-pitch Helix (VB.NET)](Create_and_Modify_Variable-pitch_Helix_Example_VBNET.htm)

[Create and Modify Variable-pitch Helix (VBA)](Create_and_Modify_Variable-pitch_Helix_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create and insert a variable-pitch helix, call:

1. IFeatureManager::InsertVariablePitchHelix to create it.- [IFeatureManager::AddVariablePitchHelixFirstPitchAndDiamenter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddVariablePitchHelixFirstPitchAndDiameter.html) to add the first segment.- [IFeatureManager::AddVariablePitchHelixSegment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddVariablePitchHelixSegment.html) one or more times to add the remaining segments.- [IFeatureManager::EndVariablePitchHelix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~EndVariablePitchHelix.html) to insert it.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IHelixFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0