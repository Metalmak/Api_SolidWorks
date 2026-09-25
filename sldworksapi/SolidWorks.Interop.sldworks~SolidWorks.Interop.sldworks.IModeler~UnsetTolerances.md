<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~UnsetTolerances.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UnsetTolerances Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : UnsetTolerances Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ToleranceIDArray*
:   Array specifying the tolerances to reset as defined in swTolerances\_e

*NumTol*
:   Number of tolerance types you are resetting; this value should correspond to the number of elements in the ToleranceIDArray array

Sets the tolerances back to system settings.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UnsetTolerances( _    ByRef ToleranceIDArray As System.Integer, _    ByVal NumTol As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim ToleranceIDArray As System.Integer Dim NumTol As System.Integer Dim value As System.Boolean   value = instance.UnsetTolerances(ToleranceIDArray, NumTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UnsetTolerances(     ref System.int ToleranceIDArray,    System.int NumTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool UnsetTolerances(  &   System.int% ToleranceIDArray, &   System.int NumTol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ToleranceIDArray*
:   Array specifying the tolerances to reset as defined in swTolerances\_e

*NumTol*
:   Number of tolerance types you are resetting; this value should correspond to the number of elements in the ToleranceIDArray array

#### Return Value

True if the tolerances is reset successfully, false if n

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::UnsetTolerances.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::GetToleranceValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~GetToleranceValue.html)

[IModeler::SetToleranceValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SetToleranceValue.html)