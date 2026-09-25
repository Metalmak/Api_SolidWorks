<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData~ISetComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetComponents Method (ICavityFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICavityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html) : ISetComponents Method (ICavityFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of design components

*Comps*
:   * in-process, unmanaged C++: Pointer to an array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) objects of size Count

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Sets the design components for this cavity feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ISetComponents( _    ByVal Count As System.Integer, _    ByRef Comps As Component2 _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICavityFeatureData Dim Count As System.Integer Dim Comps As Component2   instance.ISetComponents(Count, Comps) ``` | |

| C# |  |
| --- | --- |
| ``` void ISetComponents(     System.int Count,    ref Component2 Comps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ISetComponents(  &   System.int Count, &   Component2^% Comps ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of design components

*Comps*
:   * in-process, unmanaged C++: Pointer to an array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) objects of size Count

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CavityFeatureData::ISetComponents.

# ![](dotnetimages/collapse.gif)Remarks

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICavityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html)

[ICavityFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData_members.html)

[ICavityFeatureData::IGetComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData~IGetComponents.html)

[ICavityFeatureData::GetComponentsCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData~GetComponentsCount.html)

[ICavityFeatureData::Components Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData~Components.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13