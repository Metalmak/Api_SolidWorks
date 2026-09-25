<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetSelections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetSelections2 Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : IGetSelections2 Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SelCount*

*Objects*

*ObjectTypes*

*SelMarks*

*DrViews*

Obsolete. Superseded by [IMacroFeatureData::IGetSelections3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IGetSelections3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetSelections2( _    ByVal SelCount As System.Integer, _    ByRef Objects As System.Object, _    ByRef ObjectTypes As System.Integer, _    ByRef SelMarks As System.Integer, _    ByRef DrViews As View _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim SelCount As System.Integer Dim Objects As System.Object Dim ObjectTypes As System.Integer Dim SelMarks As System.Integer Dim DrViews As View   instance.IGetSelections2(SelCount, Objects, ObjectTypes, SelMarks, DrViews) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetSelections2(     System.int SelCount,    out System.object Objects,    out System.int ObjectTypes,    out System.int SelMarks,    out View DrViews ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetSelections2(  &   System.int SelCount, &   [Out] System.Object^ Objects, &   [Out] System.int ObjectTypes, &   [Out] System.int SelMarks, &   [Out] View^ DrViews ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SelCount*

*Objects*

*ObjectTypes*

*SelMarks*

*DrViews*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MacroFeatureData::IGetSelections2.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)