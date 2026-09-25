<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IStructureSystemFolder Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IStructureSystemFolder Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a structure system folder.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IStructureSystemFolder ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStructureSystemFolder ``` | |

| C# |  |
| --- | --- |
| ``` public interface IStructureSystemFolder ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IStructureSystemFolder ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StructureSystemFolder.

# ![](dotnetimages/collapse.gif)Example

See the [IPrimaryMemberFacePlaneIntersectionFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData.html) examples.

See the [IPrimaryMemberPointLengthFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData.html) examples.

See the [IPrimaryMemberPathSegmentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData.html) examples.

See the [IPrimaryMemberRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData.html) examples.

See the [ISecondaryMemberBetweenPointsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This interface accesses the top-level folder of a structure system in the FeatureManager design tree. The structure system folder contains one or more profile group folders. Each profile group folder contains profile references and structure system members.

A structure system appears as follows in the FeatureManager design tree. In parentheses are the APIs that you use to access the item:

- **Structure System1** (IStructureSystemFolder accessors)

  - **Structure System Grid1**

  - **<ansi inch> <c channel><3 x 5> (1)** ([IProfileGroupFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder.html) accessors)

     - **Plane2** (profile reference plane - [IProfileGroupFolder::GetPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetPlane.html))

     - **Sketch11** (profile sketch - [IProfileGroupFolder::GetSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetSketch.html))

     - **Member1** (structure system member - [IProfileGroupFolder::GetStructureSystemMembers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder~GetStructureSystemMembers.html))

To create a structure system:

1. Create an [IStructureSystemMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData.html) object for every primary and secondary structure system member you intend to create.- Create [IStructureSystemSplitMember](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemSplitMember.html) objects as needed. Use [IStructureSystemMemberFeatureData::IsSplit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~IsSplit.html) to indicate that split members exist.- Create one or more [IStructureSystemMemberProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberProfile.html) objects as the number of different profiles is needed.- Cast the IStructureSystemMemberFeatureData objects to [IPrimaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryStructuralMemberFeatureData.html) objects and  [ISecondaryStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryStructuralMemberFeatureData.html) objects as needed.- Create specific primary member feature data objects by casting IPrimaryStructuralMemberFeatureData objects to:

             -  [IPrimaryMemberFacePlaneIntersectionFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberFacePlaneIntersectionFeatureData.html)
             -  [IPrimaryMemberPathSegmentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPathSegmentFeatureData.html)
             -  [IPrimaryMemberPointLengthFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberPointLengthFeatureData.html)
             -  [IPrimaryMemberRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrimaryMemberRefPlaneFeatureData.html)
           - Create specific secondary member feature data objects by casting ISecondaryStructuralMemberFeatureData objects to:

               -  [ISecondaryMemberBetweenPointsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html)
               -  [ISecondaryMemberSupportPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberSupportPlaneFeatureData.html)
             - Use the methods and properties on the specific primary and secondary member feature data objects to detail the structure system members.- Call [IModelDocExtension::CreateStructureSystem](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStructureSystem.html)(*primaryFDArray*, *secondaryFDArray*), where *primaryFDArray* is an array of primary IStructureSystemMemberFeatureData objects and *secondaryFDArray* is an array of secondary IStructureSystemMemberFeatureData objects created in step 1.

To edit a structure system:

1. Get the structure system folder feature, which is returned by IModelDocExtension::CreateStructureSystem in step 8 above. Then call the accessor of this interface, IFeature::GetSpecificFeature2.
   (Or call both accessors of this interface.)- Use [IStructureSystemFolder::GetProfileGroupFolders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder~GetProfileGroupFolders.html) to access the profile group folders in a structure system folder.- Use IProfileGroupFolder methods and properties to get the sketch, reference plane, and structure system members in each profile group folder.- Use [IStructureSystemMemberFeatureData::StructureSystemMemberType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~StructureSystemMemberType.html) to determine whether a structure system member retrieved in step 3 is a primary or a secondary member.- Call [IStructureSystemMemberFeatureData::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~AccessSelections.html) before editing the selections used to create the structure system. Call [IStructureSystemMemberFeatureData::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~ReleaseSelectionAccess.html) after editing.- Cast IStructureSystemMemberFeatureData objects to their subclass feature data objects (see create steps 5 and 6).- If you need to change a structure member's profile, use [IStructureSystemMemberFeatureData::MemberProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~MemberProfile.html) to get the IStructureSystemMemberProfile object for each structure member.- Complete the structure system edit by calling [IStructureSystemMemberFeatureData::GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData~GetFeature.html), calling methods and properties on objects retrieved in previous steps as required, and finally calling [IFeature::ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html).

Use the examples as models to create and edit structure sytems in your own applications.

For more information, read the **SOLIDWORKS user-interface help > Weldments and Structure System > Structure System** topics.

# ![](dotnetimages/collapse.gif)Accessors

Call [IFeatureManager::GetStructureSystemFolders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GetStructureSystemFolders.html) and then [IFeature::GetSpecificFeature2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetSpecificFeature2.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[StructureSystemFolder](SWObjectModel.pdf#StructureSystemFolder)

# ![](dotnetimages/collapse.gif)See Also

####

[IStructureSystemFolder Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)