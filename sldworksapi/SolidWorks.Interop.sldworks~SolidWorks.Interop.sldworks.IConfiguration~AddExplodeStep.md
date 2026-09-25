<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddExplodeStep Method (IConfiguration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : AddExplodeStep Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplDist*
:   Explode distance

*ReverseDir*
:   True to reverse the direction of the explode step, false to not

*RigidSubassembly*
:   True to explode entire sub assembly, false to explode just the selected component

*ExplodeRelated*
:   True to explode related components together, false to not

Obsolete. Superseded by [IConfiguration::AddExplodeStep2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AddExplodeStep2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddExplodeStep( _    ByVal ExplDist As System.Double, _    ByVal ReverseDir As System.Boolean, _    ByVal RigidSubassembly As System.Boolean, _    ByVal ExplodeRelated As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim ExplDist As System.Double Dim ReverseDir As System.Boolean Dim RigidSubassembly As System.Boolean Dim ExplodeRelated As System.Boolean Dim value As System.Object   value = instance.AddExplodeStep(ExplDist, ReverseDir, RigidSubassembly, ExplodeRelated) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddExplodeStep(     System.double ExplDist,    System.bool ReverseDir,    System.bool RigidSubassembly,    System.bool ExplodeRelated ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddExplodeStep(  &   System.double ExplDist, &   System.bool ReverseDir, &   System.bool RigidSubassembly, &   System.bool ExplodeRelated ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplDist*
:   Explode distance

*ReverseDir*
:   True to reverse the direction of the explode step, false to not

*RigidSubassembly*
:   True to explode entire sub assembly, false to explode just the selected component

*ExplodeRelated*
:   True to explode related components together, false to not

#### Return Value

Pointer to a newly created [explode step](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExplodeStep.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::AddExplodeStep.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if an explode view exists in the active configuration. To create an explode view, call [IAssemblyDoc::AutoExplode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AutoExplode.html) or [IAssemblyDoc::CreateExplodedView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateExplodedView.html).

Before calling this method, you must select by mark both a direction along which to explode and a component to move. For example:

boolstatus = Model.Extension.SelectByID2('', 'EDGE', -0.011, 0.06, 0.084, True, 1, Nothing)

boolstatus = Model.Extension.SelectByID2('squarebolt1-1@Assem1', 'COMPONENT', 0, 0, 0, True, 2, Nothing, swSelectOptionDefault)

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::IAddExplodeStep Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IAddExplodeStep.html)

[IConfiguration::DeleteExplodeStep Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~DeleteExplodeStep.html)

[IConfiguration::GetExplodeStep Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetExplodeStep.html)

[IConfiguration::GetNumberOfExplodeSteps Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetNumberOfExplodeSteps.html)

[IConfiguration::IGetExplodeStep Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IGetExplodeStep.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0