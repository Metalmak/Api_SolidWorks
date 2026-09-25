<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~GetItem2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetItem2 Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : GetItem2 Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index number of the criterion to retrieve

*Category1*
:   Name of Category1 (see **Remarks**)

*Category2*
:   Name of Category2 (see **Remarks**)

*Condition*
:   Condition as defined in swAdvSelectType\_e (see **Remarks**)

*Value*
:   Text value satisfying Condition (see **Remarks**)

*IsAnd*
:   True if all of the criteria in the advanced component selection criteria list must be met, false if only this criterion must be met

Gets the specified advanced component selection criterion.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetItem2( _    ByVal Index As System.Integer, _    ByRef Category1 As System.String, _    ByRef Category2 As System.String, _    ByRef Condition As System.Integer, _    ByRef Value As System.String, _    ByRef IsAnd As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim Index As System.Integer Dim Category1 As System.String Dim Category2 As System.String Dim Condition As System.Integer Dim Value As System.String Dim IsAnd As System.Boolean Dim value As System.Integer   value = instance.GetItem2(Index, Category1, Category2, Condition, Value, IsAnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetItem2(     System.int Index,    out System.string Category1,    out System.string Category2,    out System.int Condition,    out System.string Value,    out System.bool IsAnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetItem2(  &   System.int Index, &   [Out] System.String^ Category1, &   [Out] System.String^ Category2, &   [Out] System.int Condition, &   [Out] System.String^ Value, &   [Out] System.bool IsAnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index number of the criterion to retrieve

*Category1*
:   Name of Category1 (see **Remarks**)

*Category2*
:   Name of Category2 (see **Remarks**)

*Condition*
:   Condition as defined in swAdvSelectType\_e (see **Remarks**)

*Value*
:   Text value satisfying Condition (see **Remarks**)

*IsAnd*
:   True if all of the criteria in the advanced component selection criteria list must be met, false if only this criterion must be met

#### Return Value

Value of the Index argument or -1 if criterion specified by Index not found

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::GetItem2.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedSelectionCriteria](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call [IAdvancedSelectionCriteria::GetItemCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAdvancedSelectionCriteria~GetItemCount.html) to get a valid value for Index before calling this method.

For a list of possible Category1, Category2, Condition, and Value values, see **Assemblies > Basic Component Operations > Selecting Components > Advanced Component Selection > Search Criteria for Advanced Component Selection** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29