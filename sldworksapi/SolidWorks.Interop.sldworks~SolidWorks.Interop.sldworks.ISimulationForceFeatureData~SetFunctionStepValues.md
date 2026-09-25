<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~SetFunctionStepValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFunctionStepValues Method (ISimulationForceFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulationForceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html) : SetFunctionStepValues Method (ISimulationForceFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*F1InitialValue*
:   Value of the function before the step

*T1StartStepTime*
:   Time at which the step begins

*F2InitialValue*
:   Value of the function after the step

*T2EndStepTime*
:   Time at which the step ends

Sets the step function, whose magnitude transitions smoothly from one value to another value, for this Force feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFunctionStepValues( _    ByVal F1InitialValue As System.Double, _    ByVal T1StartStepTime As System.Double, _    ByVal F2InitialValue As System.Double, _    ByVal T2EndStepTime As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulationForceFeatureData Dim F1InitialValue As System.Double Dim T1StartStepTime As System.Double Dim F2InitialValue As System.Double Dim T2EndStepTime As System.Double Dim value As System.Boolean   value = instance.SetFunctionStepValues(F1InitialValue, T1StartStepTime, F2InitialValue, T2EndStepTime) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetFunctionStepValues(     System.double F1InitialValue,    System.double T1StartStepTime,    System.double F2InitialValue,    System.double T2EndStepTime ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetFunctionStepValues(  &   System.double F1InitialValue, &   System.double T1StartStepTime, &   System.double F2InitialValue, &   System.double T2EndStepTime ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*F1InitialValue*
:   Value of the function before the step

*T1StartStepTime*
:   Time at which the step begins

*F2InitialValue*
:   Value of the function after the step

*T2EndStepTime*
:   Time at which the step ends

#### Return Value

True if the operation succeeds, false if it fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimulationForceFeatureData::SetFunctionStepValues.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationForceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html)

[ISimulationForceFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData_members.html)

[ISimulationForceFeatureData::GetFunctionStepValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetFunctionStepValues.html)

[ISimulationForceFeatureData::GetFunctionHarmonicValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~GetFunctionHarmonicValues.html)

[ISimulationForceFeatureData::SetFunctionHarmonicValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~SetFunctionHarmonicValues.html)

[ISimulationForceFeatureData::FunctionConstantValue Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~FunctionConstantValue.html)

[ISimulationForceFeatureData::FunctionExpression Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~FunctionExpression.html)

[ISimulationForceFeatureData::ForceFunctionType Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData~ForceFunctionType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0