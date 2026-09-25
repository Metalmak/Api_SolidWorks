<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SetTolerances.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetTolerances Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : SetTolerances Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ToleranceIDArray*
:   Type of tolerance you want to set as defined in swTolerances\_e

*ToleranceValueArray*
:   New tolerance value in meters for the specified tolerance type

*NumTol*
:   Original value of the specified tolerance type

Obsolete. Superseded by [IModeler::GetToleranceValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~GetToleranceValue.html) and [IModeler::SetToleranceValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~SetToleranceValue.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTolerances( _    ByRef ToleranceIDArray As System.Integer, _    ByRef ToleranceValueArray As System.Double, _    ByVal NumTol As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim ToleranceIDArray As System.Integer Dim ToleranceValueArray As System.Double Dim NumTol As System.Integer Dim value As System.Boolean   value = instance.SetTolerances(ToleranceIDArray, ToleranceValueArray, NumTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTolerances(     ref System.int ToleranceIDArray,    ref System.double ToleranceValueArray,    System.int NumTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTolerances(  &   System.int% ToleranceIDArray, &   System.double% ToleranceValueArray, &   System.int NumTol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ToleranceIDArray*
:   Type of tolerance you want to set as defined in swTolerances\_e

*ToleranceValueArray*
:   New tolerance value in meters for the specified tolerance type

*NumTol*
:   Original value of the specified tolerance type

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::SetTolerances.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)