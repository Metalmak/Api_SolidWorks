<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddRadialExplodeStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddRadialExplodeStep Method (IConfiguration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : AddRadialExplodeStep Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplDist*
:   Distance in meters to move the components in this explode step

*ExplAng*
:   Angle in radians of rotation about component origins

*DivergeFromAxis*
:   True to move components at an angle from the selected explode direction, false to not (see **Remarks**)

*Error*
:   Error code as defined in swCreateExplodeStepError\_e

Adds a radial explode step to the explode view of the active configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddRadialExplodeStep( _    ByVal ExplDist As System.Double, _    ByVal ExplAng As System.Double, _    ByVal DivergeFromAxis As System.Boolean, _    ByRef Error As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim ExplDist As System.Double Dim ExplAng As System.Double Dim DivergeFromAxis As System.Boolean Dim Error As System.Integer Dim value As System.Object   value = instance.AddRadialExplodeStep(ExplDist, ExplAng, DivergeFromAxis, Error) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddRadialExplodeStep(     System.double ExplDist,    System.double ExplAng,    System.bool DivergeFromAxis,    out System.int Error ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddRadialExplodeStep(  &   System.double ExplDist, &   System.double ExplAng, &   System.bool DivergeFromAxis, &   [Out] System.int Error ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplDist*
:   Distance in meters to move the components in this explode step

*ExplAng*
:   Angle in radians of rotation about component origins

*DivergeFromAxis*
:   True to move components at an angle from the selected explode direction, false to not (see **Remarks**)

*Error*
:   Error code as defined in swCreateExplodeStepError\_e

#### Return Value

[Explode step](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::AddRadialExplodeStep.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Is valid only for an active current explode view. To create an explode view, call [IAssemblyDoc::AutoExplode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AutoExplode.html) or [IAssemblyDoc::CreateExplodedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateExplodedView.html).* Always clears the selection list.* Does not work if the Explode PropertyManager is open.* Does not work if any component is being edited in the context of the assembly.

Before calling this method, you must:

1. Use [IConfigurationManager::ActiveConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html) to get the active configuration for the assembly.- Call [IAssemblyDoc::ShowExploded2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ShowExploded2.html) to activate an explode view.- Call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select:

* Components to move with Mark = 1.* An explode direction entity (cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), conical face, linear [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), or [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)) with Mark = 34.* A diverge direction entity (cylindrical face, conical face, linear edge, or axis) with Mark = 64. The selected entity must form an angle with the direction entity. If DivergeFromAxis is set to true and an invalid diverge direction is selected, then DivergeFromAxis is set to false, and the direction entity is set to null. If DivergeFromAxis is set to false, then the direction entity is set to null.

After calling this method, call [IModelDoc2::EditRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRebuild3.html).

For C++, specify VARIANT\_TRUE or VARIANT\_FALSE for ReverseDir and DivergeFromAxis.

To edit a radial explode step, see the [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html) remarks.

To create an explode step for the explode view of a multibody part, see [IConfiguration::AddPartExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddPartExplodeStep.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::GetNumberOfExplodeSteps Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetNumberOfExplodeSteps.html)

[IConfiguration::GetExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetExplodeStep.html)

[IConfiguration::DeleteExplodeStep Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~DeleteExplodeStep.html)

[IConfiguration::AddExplodeStep2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0