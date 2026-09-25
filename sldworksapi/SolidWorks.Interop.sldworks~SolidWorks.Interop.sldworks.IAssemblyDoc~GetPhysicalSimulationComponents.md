<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetPhysicalSimulationComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPhysicalSimulationComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : GetPhysicalSimulationComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InDuration*
:   Total elapsed time for Physical Simulation

*OutCount*
:   Size for all returned arrays

*OutComponents*
:   Array of the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) objects

*OutTransforms*
:   Array of the [IMathTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) objects

*OutStepStartTimes*
:   Array of doubles of size outCount; when each step in the Physical Simulation should happen

*OutStepDurations*
:   Array of doubles of size outCount; how long each step in the Physical Simulation should take

*OutTotalPhysSimDuration*
:   Total elapsed time Physical Simulation should have taken

Obsolete. Not superseded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetPhysicalSimulationComponents( _    ByVal InDuration As System.Double, _    ByRef OutCount As System.Integer, _    ByRef OutComponents As System.Object, _    ByRef OutTransforms As System.Object, _    ByRef OutStepStartTimes As System.Object, _    ByRef OutStepDurations As System.Object, _    ByRef OutTotalPhysSimDuration As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim InDuration As System.Double Dim OutCount As System.Integer Dim OutComponents As System.Object Dim OutTransforms As System.Object Dim OutStepStartTimes As System.Object Dim OutStepDurations As System.Object Dim OutTotalPhysSimDuration As System.Double   instance.GetPhysicalSimulationComponents(InDuration, OutCount, OutComponents, OutTransforms, OutStepStartTimes, OutStepDurations, OutTotalPhysSimDuration) ``` | |

| C# |  |
| --- | --- |
| ``` void GetPhysicalSimulationComponents(     System.double InDuration,    out System.int OutCount,    out System.object OutComponents,    out System.object OutTransforms,    out System.object OutStepStartTimes,    out System.object OutStepDurations,    out System.double OutTotalPhysSimDuration ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetPhysicalSimulationComponents(  &   System.double InDuration, &   [Out] System.int OutCount, &   [Out] System.Object^ OutComponents, &   [Out] System.Object^ OutTransforms, &   [Out] System.Object^ OutStepStartTimes, &   [Out] System.Object^ OutStepDurations, &   [Out] System.double OutTotalPhysSimDuration ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InDuration*
:   Total elapsed time for Physical Simulation

*OutCount*
:   Size for all returned arrays

*OutComponents*
:   Array of the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) objects

*OutTransforms*
:   Array of the [IMathTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) objects

*OutStepStartTimes*
:   Array of doubles of size outCount; when each step in the Physical Simulation should happen

*OutStepDurations*
:   Array of doubles of size outCount; how long each step in the Physical Simulation should take

*OutTotalPhysSimDuration*
:   Total elapsed time Physical Simulation should have taken

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::GetPhysicalSimulationComponents.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[ISimulation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation.html)

[ISimulationGravityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationGravityFeatureData.html)

[ISimulationLinearSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html)

[ISimulationMotorFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12