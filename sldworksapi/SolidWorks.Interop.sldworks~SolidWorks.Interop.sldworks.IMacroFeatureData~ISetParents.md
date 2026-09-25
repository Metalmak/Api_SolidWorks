<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetParents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetParents Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : ISetParents Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ParentCount*
:   Number of parent features for this macro feature

*PFeatures*
:   * in-process, unmanaged C++: Pointer to an array of parent [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Sets the parent features for this macro feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ISetParents( _    ByVal ParentCount As System.Integer, _    ByRef PFeatures As Feature _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim ParentCount As System.Integer Dim PFeatures As Feature   instance.ISetParents(ParentCount, PFeatures) ``` | |

| C# |  |
| --- | --- |
| ``` void ISetParents(     System.int ParentCount,    ref Feature PFeatures ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ISetParents(  &   System.int ParentCount, &   Feature^% PFeatures ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ParentCount*
:   Number of parent features for this macro feature

*PFeatures*
:   * in-process, unmanaged C++: Pointer to an array of parent [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MacroFeatureData::ISetParents.

# ![](dotnetimages/collapse.gif)Remarks

Parent features set by this method are not persistent when the macro feature is regenerated. Reset the parent features in the SwComFeature::Regenerate handler.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

[IMacroFeatureData::GetParentsCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetParentsCount.html)

[IMacroFeatureData::IGetParents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetParents.html)

[IMacroFeatureData::Parents Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~Parents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0