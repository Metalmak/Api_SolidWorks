<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~LoadCriteria.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LoadCriteria Method (IAdvancedSelectionCriteria) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) : LoadCriteria Method (IAdvancedSelectionCriteria) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CriteriaFileName*
:   Path and filename of query file (see **Remarks**)

Loads the specified query file and makes it the current advanced component selection criteria list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function LoadCriteria( _    ByVal CriteriaFileName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria Dim CriteriaFileName As System.String Dim value As System.Boolean   value = instance.LoadCriteria(CriteriaFileName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool LoadCriteria(     System.string CriteriaFileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool LoadCriteria(  &   System.String^ CriteriaFileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CriteriaFileName*
:   Path and filename of query file (see **Remarks**)

#### Return Value

True if query file loads, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria::LoadCriteria.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedSelectionCriteria](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Specify CriteriaFileName with either a **\*.xml** file or a legacy **\*.sqy** file.

To create a **\*.xml** query file, you can either:

* Use the Advanced Component Selection dialog (**Standard toolbar > Advanced Select**) to export a query file in XML format.

    - or -

* Open a txt file in Notepad and add content as follows:

<?xml version="1.0" encoding="UTF-8"?>
<SWQueryList>
    <Query Name="InContextHasMate" Favourites\_Index="1">
     <Boolean Name="And" Category="In Context Relations" SubCategory="Has mate to part" Condition="=" Value="base plate-1@98food processor"/>
 </Query>
</SWQueryList>

1. Replace the attribute values in the <Query> and <Boolean> elements as required. Refer to the **Assemblies > Basic Component Operations > Selecting Components > Advanced Component Selection > Search Criteria for Advanced Component Selection** topic in the SOLIDWORKS help to see all the options for populating the Category (Category1 in the dialog), SubCategory (Category2 in the dialog), Condition, and Value attributes.- In <Query> Favourites\_Index specifies where the query appears at the end of the Select toolbar. This attribute corresponds to the row number in the Manage Searches tab of the dialog.- In <Boolean> Name specifies "And" (default) or "Or" to indicate whether to logically AND or OR multiple Boolean elements in the Query element. This attribute corresponds to the And/Or column in the dialog.- Add more <Query> and <Boolean> elements as needed to further constrain your query.- Save the query file with a **.xml** extension.

After calling this method, call [IAdvancedSelectionCriteria::Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~Select.html) to select the assembly components that satisfy the query criteria.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html)

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14