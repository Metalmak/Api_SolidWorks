<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPartExplodeStep Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPartExplodeStep Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the explode step of an explode view of a multibody part.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPartExplodeStep ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartExplodeStep ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPartExplodeStep ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPartExplodeStep ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartExplodeStep.

# ![](dotnetimages/collapse.gif)Example

[Add Multibody Part Explode Step (VBA)](Add_Multibody_Part_Explode_Step_Example.htm)

[Add Multibody Part Explode Step (VB.NET)](Add_Multibody_Part_Explode_Step_Example_VBNET.htm)

[Add Multibody Part Explode Step (C#)](Add_Multibody_Part_Explode_Step_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface is valid only for an active current explode view of a multibody part. To create an explode view of a multibody part, call [IPartDoc::CreateExplodedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~CreateExplodedView.html).

The setter properties and methods of this interface:

* Always clear selection lists.* Do not work if the Explode PropertyManager is open.* Do not work if any body is being edited in the context of the multibody part.

To edit an explode step:

1. Use [IPartDoc::ShowExploded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ShowExploded.html) to activate the explode view of interest.- Use [IPartDoc::GetExplodedViewConfigurationName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~GetExplodedViewConfigurationName.html) to get the configuration for the explode view.- Call [IConfiguration::GetPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetPartExplodeStep.html) to access the explode step of interest.- Call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select:
         1. Bodies to move with Mark = 1.- An explode direction entity (cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), conical face, linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), or [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)) with Mark = 2.- Call [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html) to get the bodies selected in step 4a.- Call [IPartExplodeStep::SetBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep~SetBodies.html), passing in the bodies gotten in step 4a.- Call [IPartExplodeStep::SetExplodeDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep~SetExplodeDirection.html), passing in the explode direction entity that was selected in step 4b. See **Notes**.- Modify other explode step properties.

**Notes**:

When editing the object entity for the explode direction, please bear in mind:

| If... | Then... |
| --- | --- |
| Both object and manipulator index are valid | Both object and manipulator index are set. |
| Manipulator index is valid, but object is invalid | Manipulator index is set, and object is unchanged. |
| Object is valid, but manipulator index is invalid | Object is set, and the manipulator index is reset to the Z direction index. |
| Both object and manipulator index are invalid | No values change. |

For more information, see **Exploded Views in Multibody Parts** topic in the SOLIDWORKS user-interface help.

To access explode steps of explode views of assemblies, see [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html).

# ![](dotnetimages/collapse.gif)Accessors

[IConfiguration::AddPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddPartExplodeStep.html)

IConfiguration::GetPartExplodeStep

# ![](dotnetimages/collapse.gif)Access Diagram

[PartExplodeStep](SWObjectModel.pdf#PartExplodeStep)

# ![](dotnetimages/collapse.gif)See Also

####

[IPartExplodeStep Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)