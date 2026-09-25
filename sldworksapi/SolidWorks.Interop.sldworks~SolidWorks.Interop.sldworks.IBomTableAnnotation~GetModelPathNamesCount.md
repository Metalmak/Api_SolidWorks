<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNamesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModelPathNamesCount Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : GetModelPathNamesCount Method (IBomTableAnnotation) |

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

Gets the number of model pathnames in the specified row of this BOM table annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetModelPathNamesCount( _    ByVal RowIndex As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim RowIndex As System.Integer Dim value As System.Integer   value = instance.GetModelPathNamesCount(RowIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetModelPathNamesCount(     System.int RowIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetModelPathNamesCount(  &   System.int RowIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowIndex*
:   Row in the BOM table; 0-based index

#### Return Value

Number of model pathnames in the specified row

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::GetModelPathNamesCount.

# ![](dotnetimages/collapse.gif)Example

[Get Model Pathnames in BOM Table (C#)](Get_Model_Path_Names_in_BOM_Table_Example_CSharp.htm)

[Get Model Pathnames in BOM Table (VB.NET)](Get_Model_Path_Names_in_BOM_Table_Example_VBNET.htm)

[Get Model Pathnames in BOM Table (VBA)](Get_Model_Path_Names_in_BOM_Table_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IBomTableAnnotation::IGetModelPathNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~IGetModelPathNames.html) to determine the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::GetModelPathNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP01, Revision Number 19.1