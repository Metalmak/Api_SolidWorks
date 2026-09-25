<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IExplodeStep Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IExplodeStep Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to an explode step in the explode view of the active assembly configuration.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IExplodeStep ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExplodeStep ``` | |

| C# |  |
| --- | --- |
| ``` public interface IExplodeStep ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IExplodeStep ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExplodeStep.

# ![](dotnetimages/collapse.gif)Example

[Add Regular Explode Step (VBA)](Add_Explode_Step_Example_VB.htm)

[Edit Radial Explode Step (VBA)](Edit_Radial_Explode_Step_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface is valid only for assemblies. To access the explode steps of an explode view of multibody parts, see [IPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html).

If this is a subassembly explode step, then you can call only one method on this interface, [IExplodeStep::GetSubAssemblyExplodeSteps](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetSubAssemblyExplodeSteps.html), to retrieve the nested explode steps of this subassembly explode step.

The setter properties and methods of this interface:

* Always clear selection lists.* Do not work if the Explode PropertyManager is open.* Do not work if any component is being edited in the context of the assembly.

To edit an explode step that is not a subassembly explode step:

1. Use [IConfigurationManager::ActiveConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html) to get the active configuration of the assembly.- Access the explode step. See the **Accessors** section.- Call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select:
       1. Components to move with Mark = 1.- An explode direction entity (cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), conical face, linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), or [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)) with Mark = 2 (regular explode steps) or Mark = 34 (radial explode steps).- A rotation axis with Mark = 32, if RotateAboutOrigin is set to false (regular explode steps only).- A diverge direction entity with Mark = 64 (radial explode steps only).- Call [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html) to get the components selected in step 3a.- Call [IExplodeStep::SetComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetComponents.html), passing in the components gotten in step 4.- Call [IExplodeStep::SetExplodeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetExplodeDirection.html), passing in the explode direction entity that was selected in step 3b. See **Notes**.- Call [IExplodeStep::SetRotationAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetRotationAxis.html), passing in the rotation axis that was selected in step 3c (for regular explode steps only).- Set [IExplodeStep::DivergeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~DivergeDirection.html) to the diverge direction entity that was selected in step 3d (for radial explode steps only). See **Notes**.- Modify other explode step properties.

**Notes**:

When editing the object entity for the explode direction or rotation axis, please bear in mind:

| If... | Then... |
| --- | --- |
| Both object and manipulator index are valid | Both object and manipulator index are set. |
| Manipulator index is valid, but object is invalid | Manipulator index is set, and object is unchanged. |
| Object is valid, but manipulator index is invalid | Object is set, but the manipulator index is reset to:   * Z direction index for explode direction.* XY ring index for rotation axis. |
| Both object and manipulator index are invalid | No values change. |

When editing the diverge direction object entity or the diverge from axis flag, please bear in mind:

| If... | Then... |
| --- | --- |
| Diverge direction object is valid | IExplodeStep::DivergeDirection properly sets the diverge direction, and [IExplodeStep::DivergeFromAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~DivergeFromAxis.html) is set to true. |
| Diverge direction object is null | IExplodeStep::DivergeDirection is set to null, and IExplodeStep::DivergeFromAxis is set to false. |
| Diverge direction object is invalid | Direction object entity is unchanged. |
| IExplodeStep::DivergeFromAxis is set to false | IExplodeStep::DivergeFromAxis is set to false, and the diverge direction object is set to null. |
| IExplodeStep::DivergeFromAxis is set to true | No values change. |

# ![](dotnetimages/collapse.gif)Accessors

[IConfiguration::AddExplodeStep2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep2.html)

[IConfiguration::AddRadialExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddRadialExplodeStep.html)

[IConfiguration::GetExplodeStep](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration~GetExplodeStep.html) and [IConfiguration::IGetExplodeStep](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration~IGetExplodeStep.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[ExplodeStep](SWObjectModel.pdf#ExplodeStep)

# ![](dotnetimages/collapse.gif)See Also

####

[IExplodeStep Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IAssemblyDoc::ShowExploded Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ShowExploded.html)

[IModelDoc2::IsExploded Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IsExploded.html)