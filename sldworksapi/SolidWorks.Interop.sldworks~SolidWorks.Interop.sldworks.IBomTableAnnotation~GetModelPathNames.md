<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModelPathNames Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : GetModelPathNames Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RowIndex*
:   Row in the BOM table; 0-based index

*ItemNumber*
:   Item number for the specified BOM table row

*PartNumber*
:   Part number for the specified BOM table row

Gets the full pathnames of all documents in the specified row of this BOM table annotation. Also gets the item and part numbers associated with the specified row.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetModelPathNames( _    ByVal RowIndex As System.Integer, _    ByRef ItemNumber As System.String, _    ByRef PartNumber As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim RowIndex As System.Integer Dim ItemNumber As System.String Dim PartNumber As System.String Dim value As System.Object   value = instance.GetModelPathNames(RowIndex, ItemNumber, PartNumber) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetModelPathNames(     System.int RowIndex,    out System.string ItemNumber,    out System.string PartNumber ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetModelPathNames(  &   System.int RowIndex, &   [Out] System.String^ ItemNumber, &   [Out] System.String^ PartNumber ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowIndex*
:   Row in the BOM table; 0-based index

*ItemNumber*
:   Item number for the specified BOM table row

*PartNumber*
:   Part number for the specified BOM table row

#### Return Value

Array of full pathnames of the models in the specified BOM table row

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::GetModelPathNames.

# ![](dotnetimages/collapse.gif)Example

[Get Model Pathnames in BOM Table (C#)](Get_Model_Path_Names_in_BOM_Table_Example_CSharp.htm)

[Get Model Pathnames in BOM Table (VB.NET)](Get_Model_Path_Names_in_BOM_Table_Example_VBNET.htm)

[Get Model Pathnames in BOM Table (VBA)](Get_Model_Path_Names_in_BOM_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::IGetModelPathNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetModelPathNames.html)

[IBomTableAnnotation::GetModelPathNamesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNamesCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP01, Revision Number 19.1