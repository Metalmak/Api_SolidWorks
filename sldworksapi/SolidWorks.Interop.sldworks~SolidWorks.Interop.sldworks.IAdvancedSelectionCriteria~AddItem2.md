<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~AddItem2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddItem2 Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : AddItem2 Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Category1*
:   Name of Category1 (see **Remarks**)

*Category2*
:   Name of Category2 (see **Remarks**)

*Condition*
:   Condition as defined in swAdvSelectType\_e (see **Remarks**)

*Value*
:   Text value satisfying Condition (see **Remarks**)

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list must be met

Adds the specified advanced component selection criterion to the list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddItem2( _    ByVal Category1 As System.String, _    ByVal Category2 As System.String, _    ByVal Condition As System.Integer, _    ByVal Value As System.String, _    ByVal IsAnd As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim Category1 As System.String Dim Category2 As System.String Dim Condition As System.Integer Dim Value As System.String Dim IsAnd As System.Boolean Dim value As System.Integer   value = instance.AddItem2(Category1, Category2, Condition, Value, IsAnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddItem2(     System.string Category1,    System.string Category2,    System.int Condition,    System.string Value,    System.bool IsAnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddItem2(  &   System.String^ Category1, &   System.String^ Category2, &   System.int Condition, &   System.String^ Value, &   System.bool IsAnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Category1*
:   Name of Category1 (see **Remarks**)

*Category2*
:   Name of Category2 (see **Remarks**)

*Condition*
:   Condition as defined in swAdvSelectType\_e (see **Remarks**)

*Value*
:   Text value satisfying Condition (see **Remarks**)

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list must be met

#### Return Value

Index number of the newly added criterion in the advanced component selection criteria list

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::AddItem2.

# ![](dotnetimages/collapse.gif)Remarks

For a list of possible Category1, Category2, Condition, and Value values, see the **Assemblies > Basic Component Operations > Selecting Components > Advanced Component Selection > Search Criteria for Advanced Component Selection** topic in the SOLIDWORKS user-interface help.

After calling this method multiple times to add criteria:

* [Save](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~SaveCriteria.html) the criteria.* [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~Select.html) the components satisfying the criteria.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29