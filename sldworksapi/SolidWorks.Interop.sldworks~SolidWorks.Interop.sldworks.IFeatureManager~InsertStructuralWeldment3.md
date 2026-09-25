<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertStructuralWeldment3 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertStructuralWeldment3 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Path, filename, and name of the type of structural member to insert

*EndCond*
:   End condition as defined in swSOLIDWORKSWeldmentEndCondOptions\_e

*Angle*
:   Angle of rotation of the sketch about the sketch segment

*Merge*
:   True to merge the bodies of the arc segments to the adjacent bodies, false to not

*Groups*
:   :   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html)

Obsolete. Superseded by [IFeatureManager::InsertStructuralWeldment4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertStructuralWeldment4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertStructuralWeldment3( _    ByVal Path As System.String, _    ByVal EndCond As System.Integer, _    ByVal Angle As System.Double, _    ByVal Merge As System.Boolean, _    ByVal Groups As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Path As System.String Dim EndCond As System.Integer Dim Angle As System.Double Dim Merge As System.Boolean Dim Groups As System.Object Dim value As Feature   value = instance.InsertStructuralWeldment3(Path, EndCond, Angle, Merge, Groups) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertStructuralWeldment3(     System.string Path,    System.int EndCond,    System.double Angle,    System.bool Merge,    System.object Groups ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertStructuralWeldment3(  &   System.String^ Path, &   System.int EndCond, &   System.double Angle, &   System.bool Merge, &   System.Object^ Groups ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Path, filename, and name of the type of structural member to insert

*EndCond*
:   End condition as defined in swSOLIDWORKSWeldmentEndCondOptions\_e

*Angle*
:   Angle of rotation of the sketch about the sketch segment

*Merge*
:   True to merge the bodies of the arc segments to the adjacent bodies, false to not

*Groups*
:   :   Array of [IStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberGroup.html)

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertStructuralWeldment3.

# ![](dotnetimages/collapse.gif)Example

[Insert Weldment Features (VBA)](Insert_Weldment_Features_Example_VB.htm)

[Insert Weldment Features (VB.NET)](Insert_Weldment_Features_Example_VBNET.htm)

[Create Structural-Member Group (VBA)](Create_Structural_Member_Group_Example_VB.htm)

[Create Structural-Member Group (VB.NET)](Create_Structural_Member_Group_Example_VBNET.htm)

[Create Structural-Member Group (C#)](Create_Structural_Member_Group_Example_CSharp.htm)

[Insert Weldment Features (C#)](Insert_Weldment_Features_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IFeatureManager::CreateStructuralMemberGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~CreateStructuralMemberGroup.html), [IStructuralMemberFeatureData::Groups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~Groups.html), or [IStructuralMemberFeatureData::IGetGroups](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStructuralMemberFeatureData~IGetGroups.html) to populate the *Groups* parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html)

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP5, Revision Number 17.5