<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddPartExplodeStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddPartExplodeStep Method (IConfiguration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : AddPartExplodeStep Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplodeView*
:   Name of the explode view to which to add this explode step

*ExplDist*
:   Distance in meters to move the selected bodies in this explode step

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e (see **Remarks**)

*ReverseDir*
:   True to reverse the explode direction, false to not

*AutoSpaceBodiesOnDrag*
:   True to automatically space selected bodies on drag, false to not

*Error*
:   Error code as defined in swCreatePartExplodeStepError\_e

Adds an explode step to the specified explode view of a multibody part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddPartExplodeStep( _    ByVal ExplodeView As System.String, _    ByVal ExplDist As System.Double, _    ByVal ExplDirIndex As System.Integer, _    ByVal ReverseDir As System.Boolean, _    ByVal AutoSpaceBodiesOnDrag As System.Boolean, _    ByRef Error As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim ExplodeView As System.String Dim ExplDist As System.Double Dim ExplDirIndex As System.Integer Dim ReverseDir As System.Boolean Dim AutoSpaceBodiesOnDrag As System.Boolean Dim Error As System.Integer Dim value As System.Object   value = instance.AddPartExplodeStep(ExplodeView, ExplDist, ExplDirIndex, ReverseDir, AutoSpaceBodiesOnDrag, Error) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddPartExplodeStep(     System.string ExplodeView,    System.double ExplDist,    System.int ExplDirIndex,    System.bool ReverseDir,    System.bool AutoSpaceBodiesOnDrag,    out System.int Error ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddPartExplodeStep(  &   System.String^ ExplodeView, &   System.double ExplDist, &   System.int ExplDirIndex, &   System.bool ReverseDir, &   System.bool AutoSpaceBodiesOnDrag, &   [Out] System.int Error ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplodeView*
:   Name of the explode view to which to add this explode step

*ExplDist*
:   Distance in meters to move the selected bodies in this explode step

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e (see **Remarks**)

*ReverseDir*
:   True to reverse the explode direction, false to not

*AutoSpaceBodiesOnDrag*
:   True to automatically space selected bodies on drag, false to not

*Error*
:   Error code as defined in swCreatePartExplodeStepError\_e

#### Return Value

[IPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::AddPartExplodeStep.

# ![](dotnetimages/collapse.gif)Example

See the [IPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Is valid only for an active, current explode view of a multibody part.* Always clears the selection list.* Does not work if the Explode PropertyManager is open.* Does not work if any body is being edited in the context of the part.

Before calling this method, you must:

1. Create an explode view in the active, current configuration of the multibody part. To create an explode view, call [IPartDoc::CreateExplodedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~CreateExplodedView.html).- Populate ExplodeView with [IConfiguration::GetCurrentPartExplodeViewName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetCurrentPartExplodeViewName.html).- Call [IPartDoc::ShowExploded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ShowExploded.html) to activate the explode view to which to add an explode step.- Call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select:

* Bodies to move with Mark = 1.* (Optionally) An explode direction entity (cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), conical face, linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), or [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)) with Mark = 2. Either, both, or neither of the direction entity and ExplDirIndex can be set. If neither, then the Z-direction manipulator index is used.

After calling this method, call [IModelDoc2::EditRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRebuild3.html).

For C++, specify VARIANT\_TRUE or VARIANT\_FALSE for ReverseDir.

To edit an explode step, see the [IPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html) remarks.

To create an explode step for the explode view of an assembly, see [IConfiguration::AddExplodeStep2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep2.html) and [IConfiguration::AddRadialExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddRadialExplodeStep.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::DeleteExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~DeleteExplodeStep.html)

[IConfiguration::GetNumberOfPartExplodeSteps Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetNumberOfPartExplodeSteps.html)

[IConfiguration::GetPartExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetPartExplodeStep.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0