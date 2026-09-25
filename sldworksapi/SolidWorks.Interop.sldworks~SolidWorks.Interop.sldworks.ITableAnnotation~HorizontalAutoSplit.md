<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~HorizontalAutoSplit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| HorizontalAutoSplit Method (ITableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html) : HorizontalAutoSplit Method (ITableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MaxNumberOfRows*
:   Maximum number of rows in the split portions

*Apply*
:   How often to horizontally split the table as defined in swHorizontalAutoSplitApply\_e

*PlacementOfNewSplitTables*
:   Where to place the horizontally split table as defined in swHorizontalAutoSplitPlacementOfSplitTable\_e

Starts the automatic horizontal splitting of this table using the specified options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function HorizontalAutoSplit( _    ByVal MaxNumberOfRows As System.Integer, _    ByVal Apply As System.Integer, _    ByVal PlacementOfNewSplitTables As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITableAnnotation Dim MaxNumberOfRows As System.Integer Dim Apply As System.Integer Dim PlacementOfNewSplitTables As System.Integer Dim value As System.Object   value = instance.HorizontalAutoSplit(MaxNumberOfRows, Apply, PlacementOfNewSplitTables) ``` | |

| C# |  |
| --- | --- |
| ``` System.object HorizontalAutoSplit(     System.int MaxNumberOfRows,    System.int Apply,    System.int PlacementOfNewSplitTables ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ HorizontalAutoSplit(  &   System.int MaxNumberOfRows, &   System.int Apply, &   System.int PlacementOfNewSplitTables ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MaxNumberOfRows*
:   Maximum number of rows in the split portions

*Apply*
:   How often to horizontally split the table as defined in swHorizontalAutoSplitApply\_e

*PlacementOfNewSplitTables*
:   Where to place the horizontally split table as defined in swHorizontalAutoSplitPlacementOfSplitTable\_e

#### Return Value

Array of split [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TableAnnotation::HorizontalAutoSplit.

# ![](dotnetimages/collapse.gif)Remarks

This method horizontally splits:

* [Hole tables](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IHoleTableAnnotation.html)* [Bill of Materials tables](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation.html)* [General tables](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGeneralTableAnnotation.html)

If Apply is set to swHorizontalAutoSplitApply\_e.Continuously, in order to stop the automatic splitting of tables, you must set [ITableAnnotation::StopAutoSplitting](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~StopAutoSplitting.html) to true.

# ![](dotnetimages/collapse.gif)See Also

####

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)

[ITableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation_members.html)

[ITableAnnotation::Split Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~Split.html)

[ITableAnnotation::GetSplitInformation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation~GetSplitInformation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0