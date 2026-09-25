<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~SaveCriteria.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveCriteria Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : SaveCriteria Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CriteriaFileName*
:   Path and filename (**\*.xml**) to which to save the current query

Saves the current query to the specified XML file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveCriteria( _    ByVal CriteriaFileName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim CriteriaFileName As System.String Dim value As System.Boolean   value = instance.SaveCriteria(CriteriaFileName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveCriteria(     System.string CriteriaFileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveCriteria(  &   System.String^ CriteriaFileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CriteriaFileName*
:   Path and filename (**\*.xml**) to which to save the current query

#### Return Value

True if current query is saved successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::SaveCriteria.

# ![](dotnetimages/collapse.gif)Remarks

Call this method after [adding](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~AddItem2.html) criteria to the current advanced component selection criteria list.

As of SOLIDWORKS 2021, you can save queries only in XML format.

As is done using the Advanced Component Selection dialog (**Standard toolbar > Advanced Select**), this method creates a query file in XML format with one or more <Query> and <Boolean> elements. Each <Query> element represents a particular search by Category (Category1 in the user interface) and SubCategory (Category2 in the user interface) to satisfy a Condition expression:

?xml version="1.0" encoding="UTF-8"?>
<SWQueryList>
   <Query Name="SelectPegs" Favourites\_Index="1">
      <Boolean Name="And" Category="Custom Property" SubCategory="IsPeg" Condition="=" Value="Yes"/>
   </Query>
   <Query Name="SelectBlockParts" Favourites\_Index="2">
      <Boolean Name="And" Category="Custom Property" SubCategory="IsBlockPart" Condition="=" Value="Yes"/>
   </Query>
</SWQueryList>

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14