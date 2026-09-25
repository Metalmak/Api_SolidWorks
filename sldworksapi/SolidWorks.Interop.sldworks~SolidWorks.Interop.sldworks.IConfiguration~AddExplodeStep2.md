<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddExplodeStep2 Method (IConfiguration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : AddExplodeStep2 Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplDist*
:   Distance in meters to move the components in this explode step

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e (see **Remarks**)

*ReverseDir*
:   True to reverse the explode direction, false to not

*ExplAng*
:   Angle in radians of component rotation (see **Remarks**)

*RotAxisIndex*
:   Rotation manipulator index as defined in swRotationAxisIndex\_e (see **Remarks**)

*ReverseAng*
:   True to reverse the direction of ExplAng, false to not

*RotateAboutOrigin*
:   True if each component rotates about its origin, false if not (see **Remarks**)

*AutoSpaceComponentsOnDrag*
:   True to automatically space components on drag, false to not (see **Remarks**)

*Error*
:   Error code as defined in swCreateExplodeStepError\_e

Adds a regular (translate and rotate) explode step to the explode view of the active configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddExplodeStep2( _    ByVal ExplDist As System.Double, _    ByVal ExplDirIndex As System.Integer, _    ByVal ReverseDir As System.Boolean, _    ByVal ExplAng As System.Double, _    ByVal RotAxisIndex As System.Integer, _    ByVal ReverseAng As System.Boolean, _    ByVal RotateAboutOrigin As System.Boolean, _    ByVal AutoSpaceComponentsOnDrag As System.Boolean, _    ByRef Error As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim ExplDist As System.Double Dim ExplDirIndex As System.Integer Dim ReverseDir As System.Boolean Dim ExplAng As System.Double Dim RotAxisIndex As System.Integer Dim ReverseAng As System.Boolean Dim RotateAboutOrigin As System.Boolean Dim AutoSpaceComponentsOnDrag As System.Boolean Dim Error As System.Integer Dim value As System.Object   value = instance.AddExplodeStep2(ExplDist, ExplDirIndex, ReverseDir, ExplAng, RotAxisIndex, ReverseAng, RotateAboutOrigin, AutoSpaceComponentsOnDrag, Error) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddExplodeStep2(     System.double ExplDist,    System.int ExplDirIndex,    System.bool ReverseDir,    System.double ExplAng,    System.int RotAxisIndex,    System.bool ReverseAng,    System.bool RotateAboutOrigin,    System.bool AutoSpaceComponentsOnDrag,    out System.int Error ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddExplodeStep2(  &   System.double ExplDist, &   System.int ExplDirIndex, &   System.bool ReverseDir, &   System.double ExplAng, &   System.int RotAxisIndex, &   System.bool ReverseAng, &   System.bool RotateAboutOrigin, &   System.bool AutoSpaceComponentsOnDrag, &   [Out] System.int Error ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplDist*
:   Distance in meters to move the components in this explode step

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e (see **Remarks**)

*ReverseDir*
:   True to reverse the explode direction, false to not

*ExplAng*
:   Angle in radians of component rotation (see **Remarks**)

*RotAxisIndex*
:   Rotation manipulator index as defined in swRotationAxisIndex\_e (see **Remarks**)

*ReverseAng*
:   True to reverse the direction of ExplAng, false to not

*RotateAboutOrigin*
:   True if each component rotates about its origin, false if not (see **Remarks**)

*AutoSpaceComponentsOnDrag*
:   True to automatically space components on drag, false to not (see **Remarks**)

*Error*
:   Error code as defined in swCreateExplodeStepError\_e

#### Return Value

[[Explode step](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html)](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExplodeStep.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::AddExplodeStep2.

# ![](dotnetimages/collapse.gif)Example

See the [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Is valid only for an active current explode view. To create an explode view, call [IAssemblyDoc::AutoExplode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AutoExplode.html) or [IAssemblyDoc::CreateExplodedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateExplodedView.html).* Always clears the selection list.* Does not work if the Explode PropertyManager is open.* Does not work if any component is being edited in the context of the assembly.

If AutoSpaceComponentsOnDrag is set to true, then RotateAboutOrigin is false and ExplAng is 0.0. Set AutoSpaceComponentsOnDrag to false to specify other values for RotateAboutOrigin and ExplAng.

Before calling this method, you must:

1. Use [IConfigurationManager::ActiveConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html) to get the active configuration for the assembly.- Call [IAssemblyDoc::ShowExploded2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ShowExploded2.html) to activate an explode view.- Call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select:

* Components to move with Mark = 1.* (Optionally) An explode direction entity (cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), conical face, linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), or [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)) with Mark = 2. Either, both, or neither of the direction entity and ExplDirIndex can be set. If neither, then the Z-direction manipulator index is used.* (Optionally) A rotation axis with Mark = 32. Valid only if RotateAboutOrigin is set to false. Either, both, or neither of the rotation axis and RotAxisIndex can be set. If neither, then the XY ring index is used.

After calling this method, call [IModelDoc2::EditRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRebuild3.html).

For C++, specify VARIANT\_TRUE or VARIANT\_FALSE for ReverseDir, ReverseAng, and RotateAboutOrigin.

To edit a regular explode step, see the [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html) remarks.

To create an explode step for the explode view of a multibody part, see [IConfiguration::AddPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddPartExplodeStep.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::AddRadialExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddRadialExplodeStep.html)

[IConfiguration::DeleteExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~DeleteExplodeStep.html)

[IConfiguration::GetExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetExplodeStep.html)

[IConfiguration::GetNumberOfExplodeSteps Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetNumberOfExplodeSteps.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0