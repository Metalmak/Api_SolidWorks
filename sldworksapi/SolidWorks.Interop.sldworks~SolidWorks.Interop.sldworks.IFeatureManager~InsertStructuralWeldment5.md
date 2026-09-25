<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertStructuralWeldment5 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertStructuralWeldment5 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Path and file name of the type of structural member (see **Remarks**)

*ConnectedSegmentsOption*
:   Option as defined in swConnectedSegmentsOption\_e

*AllowProtrusion*
:   True to allow protrusion, false to not

*Groups*
:   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html) objects

*ConfigurationName*
:   Name of the configuration in a custom weldment profile or an empty string (see **Remarks**)

Inserts a structural weldment feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertStructuralWeldment5( _    ByVal Path As System.String, _    ByVal ConnectedSegmentsOption As System.Integer, _    ByVal AllowProtrusion As System.Boolean, _    ByVal Groups As System.Object, _    ByVal ConfigurationName As System.String _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Path As System.String Dim ConnectedSegmentsOption As System.Integer Dim AllowProtrusion As System.Boolean Dim Groups As System.Object Dim ConfigurationName As System.String Dim value As Feature   value = instance.InsertStructuralWeldment5(Path, ConnectedSegmentsOption, AllowProtrusion, Groups, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertStructuralWeldment5(     System.string Path,    System.int ConnectedSegmentsOption,    System.bool AllowProtrusion,    System.object Groups,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertStructuralWeldment5(  &   System.String^ Path, &   System.int ConnectedSegmentsOption, &   System.bool AllowProtrusion, &   System.Object^ Groups, &   System.String^ ConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Path and file name of the type of structural member (see **Remarks**)

*ConnectedSegmentsOption*
:   Option as defined in swConnectedSegmentsOption\_e

*AllowProtrusion*
:   True to allow protrusion, false to not

*Groups*
:   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html) objects

*ConfigurationName*
:   Name of the configuration in a custom weldment profile or an empty string (see **Remarks**)

#### Return Value

Structural weldment [feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertStructuralWeldment5.

# ![](dotnetimages/collapse.gif)Example

[Insert Structural Weldments Using Custom Weldment Profile (C#)](Insert_Structural_Weldments_Using_Custom_Weldment_Profile_Example_CSharp.htm)

[Insert Structural Weldments Using Custom Weldment Profile (VB.NET)](Insert_Structural_Weldments_Using_Custom_Weldment_Profile_Example_VBNET.htm)

[Insert Structural Weldments Using Custom Weldment Profile (VBA)](Insert_Structural_Weldments_Using_Custom_Weldment_Profile_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Specify Path using either:

* SOLIDWORKS-supplied weldment profile (\*.**sldlfp**) from *install\_dir*\**lang**\*lang*\**weldment profiles
  -** or -* custom weldment profile (\*.**sldlfp**); see the SOLIDWORKS Help for details about custom weldment profiles

| If using... | Then specify ConfigurationName as... |
| --- | --- |
| SOLIDWORKS-supplied weldment profile | Empty string |
| Custom weldment profile | Name of the configuration in the custom weldment profile |

Use [IFeatureManager::CreateStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~CreateStructuralMemberGroup.html), [IStructuralMemberFeatureData::Groups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~Groups.html), or [IStructuralMemberFeatureData::IGetGroups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~IGetGroups.html) to populate the Groups parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html)

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

[IStructuralMemberFeatureData::ConfigurationName Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData~ConfigurationName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0