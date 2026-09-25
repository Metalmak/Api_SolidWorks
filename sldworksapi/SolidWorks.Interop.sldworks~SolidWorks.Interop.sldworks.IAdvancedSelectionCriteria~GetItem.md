<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~GetItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetItem Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : GetItem Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index number of the criteria in the advanced component selection list

*Property*
:   Name of property

*Condition*
:   Condition as defined in swAdvSelectType\_e

*Value*
:   Text of the value

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list
    must be met

Obsolete. Superseded by [IAdvancedSelectionCriteria::GetItem2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~GetItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetItem( _    ByVal Index As System.Integer, _    ByRef Property As System.String, _    ByRef Condition As System.Integer, _    ByRef Value As System.String, _    ByRef IsAnd As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim Index As System.Integer Dim Property As System.String Dim Condition As System.Integer Dim Value As System.String Dim IsAnd As System.Boolean Dim value As System.Integer   value = instance.GetItem(Index, Property, Condition, Value, IsAnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetItem(     System.int Index,    out System.string Property,    out System.int Condition,    out System.string Value,    out System.bool IsAnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetItem(  &   System.int Index, &   [Out] System.String^ Property, &   [Out] System.int Condition, &   [Out] System.String^ Value, &   [Out] System.bool IsAnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index number of the criteria in the advanced component selection list

*Property*
:   Name of property

*Condition*
:   Condition as defined in swAdvSelectType\_e

*Value*
:   Text of the value

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list
    must be met

#### Return Value

Value of the Index argument or -1 if criteria specified by Index not found

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::GetItem.

# ![](dotnetimages/collapse.gif)Example

[Use Advanced Component Selection (VBA)](Use_Advanced_Component_Selection_Example_VB.htm)

[Use Advanced Component Selection (VB.NET)](Use_Advanced_Component_Selection_Example_VBNET.htm)

[Use Advanced Component Selection (C#)](Use_Advanced_Component_Selection_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [IAdvancedSelectionCriteria::GetItemCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAdvancedSelectionCriteria~GetItemCount.html) to get a valid value for Index before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14