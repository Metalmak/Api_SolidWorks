<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertStructuralWeldment4 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertStructuralWeldment4 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Full path name of the type of structural member (see **Remarks**)

*ConnectedSegmentsOption*
:   Option as defined in swConnectedSegmentsOption\_e

*AllowProtrusion*
:   True to allow protrusion, false to not

*Groups*
:   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html)

Obsolete. Superseded by [IFeatureManager::InsertStructuralWeldment5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertStructuralWeldment4( _    ByVal Path As System.String, _    ByVal ConnectedSegmentsOption As System.Integer, _    ByVal AllowProtrusion As System.Boolean, _    ByVal Groups As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Path As System.String Dim ConnectedSegmentsOption As System.Integer Dim AllowProtrusion As System.Boolean Dim Groups As System.Object Dim value As Feature   value = instance.InsertStructuralWeldment4(Path, ConnectedSegmentsOption, AllowProtrusion, Groups) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertStructuralWeldment4(     System.string Path,    System.int ConnectedSegmentsOption,    System.bool AllowProtrusion,    System.object Groups ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertStructuralWeldment4(  &   System.String^ Path, &   System.int ConnectedSegmentsOption, &   System.bool AllowProtrusion, &   System.Object^ Groups ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Full path name of the type of structural member (see **Remarks**)

*ConnectedSegmentsOption*
:   Option as defined in swConnectedSegmentsOption\_e

*AllowProtrusion*
:   True to allow protrusion, false to not

*Groups*
:   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html)

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertStructuralWeldment4.

# ![](dotnetimages/collapse.gif)Example

[Insert Structural Weldment (C#)](Insert_Structural_Weldment_Example_CSharp.htm)

[Insert Structural Weldment (VB.NET)](Insert_Structural_Weldment_Example_VBNET.htm)

[Insert Structural Weldment (VBA)](Insert_Structural_Weldment_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Populate Path using a weldment profile (\*.**sldlfp**) from *install\_dir*\**lang**\*lang*\**weldment profiles**.

Use [IFeatureManager::CreateStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~CreateStructuralMemberGroup.html), [IStructuralMemberFeatureData::Groups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~Groups.html), or [IStructuralMemberFeatureData::IGetGroups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~IGetGroups.html) to populate the Groups parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html)

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0