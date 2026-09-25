<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetModelPathNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetModelPathNames Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : IGetModelPathNames Method (IBomTableAnnotation) |

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

*Count*
:   Number of model pathnames

*ItemNumber*
:   Item number for the specified BOM table row

*PartNumber*
:   Part number for the specified BOM table row

Gets the full pathnames of all documents in the specified row of this BOM table annotation. Also gets the item and part numbers associated with the specified row.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetModelPathNames( _    ByVal RowIndex As System.Integer, _    ByVal Count As System.Integer, _    ByRef ItemNumber As System.String, _    ByRef PartNumber As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim RowIndex As System.Integer Dim Count As System.Integer Dim ItemNumber As System.String Dim PartNumber As System.String Dim value As System.String   value = instance.IGetModelPathNames(RowIndex, Count, ItemNumber, PartNumber) ``` | |

| C# |  |
| --- | --- |
| ``` System.string IGetModelPathNames(     System.int RowIndex,    System.int Count,    out System.string ItemNumber,    out System.string PartNumber ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ IGetModelPathNames(  &   System.int RowIndex, &   System.int Count, &   [Out] System.String^ ItemNumber, &   [Out] System.String^ PartNumber ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowIndex*
:   Row in the BOM table; 0-based index

*Count*
:   Number of model pathnames

*ItemNumber*
:   Item number for the specified BOM table row

*PartNumber*
:   Part number for the specified BOM table row

#### Return Value

* in-process, unmanaged C++: Pointer to an array of model pathnames in the specified row

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IBomTableAnnotation::GetModelPathNamesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~GetModelPathNamesCount.html) to get the value of Count.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::GetModelPathNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP01, Revision Number 19.1