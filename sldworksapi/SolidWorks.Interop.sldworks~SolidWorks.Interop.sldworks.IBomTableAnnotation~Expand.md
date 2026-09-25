<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Expand.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Expand Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : Expand Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExpandType*
:   Type of item to expand as defined in swBOMTableObjectType\_e

*Index*
:   Row index; valid only if ExpandType is swBOMTableObjectType\_e.swBOMTableObjectType\_RowIndex

Expands the specified item.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Expand( _    ByVal ExpandType As System.Integer, _    ByVal Index As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim ExpandType As System.Integer Dim Index As System.Integer   instance.Expand(ExpandType, Index) ``` | |

| C# |  |
| --- | --- |
| ``` void Expand(     System.int ExpandType,    System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Expand(  &   System.int ExpandType, &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExpandType*
:   Type of item to expand as defined in swBOMTableObjectType\_e

*Index*
:   Row index; valid only if ExpandType is swBOMTableObjectType\_e.swBOMTableObjectType\_RowIndex

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::Expand.

# ![](dotnetimages/collapse.gif)Example

[Expand, Collapse, and Dissolve Subassembly in a BOM Table Example (VBA)](Dissolve_Subassembly_in_a_BOM_Table_Example_VB.htm)

[Expand, Collapse, and Dissolve Subassembly in a BOM Table Example (VB.NET)](Dissolve_Subassembly_in_a_BOM_Table_Example_VBNET.htm)

[Expand, Collapse, and Dissolve Subassembly in a BOM Table Example (C#)](Dissolve_Subassembly_in_a_BOM_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If ExpandType is swBOMTableObjectType\_e.swBOMTableObjectType\_CutList, then all cut lists in the table expand.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::Collapse Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Collapse.html)

[IBomTableAnnotation::Dissolve Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Dissolve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0