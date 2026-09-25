<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~AddItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddItem Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : AddItem Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Property*
:   Name of property

*Condition*
:   Condition as defined in swAdvSelectType\_e

*Value*
:   Text of the value

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list must be met

Obsolete. Superseded by [IAdvancedSelectionCriteria::AddItem2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~AddItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddItem( _    ByVal Property As System.String, _    ByVal Condition As System.Integer, _    ByVal Value As System.String, _    ByVal IsAnd As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim Property As System.String Dim Condition As System.Integer Dim Value As System.String Dim IsAnd As System.Boolean Dim value As System.Integer   value = instance.AddItem(Property, Condition, Value, IsAnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddItem(     System.string Property,    System.int Condition,    System.string Value,    System.bool IsAnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddItem(  &   System.String^ Property, &   System.int Condition, &   System.String^ Value, &   System.bool IsAnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Property*
:   Name of property

*Condition*
:   Condition as defined in swAdvSelectType\_e

*Value*
:   Text of the value

*IsAnd*
:   True if all of the criteria in the advanced component selection list must be met, false if only this criteria in the advanced component selection list must be met

#### Return Value

Index number of the newly added criteria in the advanced component selection list

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::AddItem.

# ![](dotnetimages/collapse.gif)Example

[Use Advanced Component Selection (VBA)](Use_Advanced_Component_Selection_Example_VB.htm)

[Use Advanced Component Selection (VB.NET)](Use_Advanced_Component_Selection_Example_VBNET.htm)

[Use Advanced Component Selection (C#)](Use_Advanced_Component_Selection_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14