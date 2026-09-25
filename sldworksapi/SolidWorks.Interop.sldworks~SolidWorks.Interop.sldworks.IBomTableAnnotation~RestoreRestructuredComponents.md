<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~RestoreRestructuredComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RestoreRestructuredComponents Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : RestoreRestructuredComponents Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RowIndex*
:   1-based row index, if more than one subassembly or weldment are dissolved; 0, if only one subassembly or weldment is dissolved

Restores the previously dissolved subassembly or weldment at the specified row index of this BOM table annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RestoreRestructuredComponents( _    ByVal RowIndex As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim RowIndex As System.Integer Dim value As System.Boolean   value = instance.RestoreRestructuredComponents(RowIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RestoreRestructuredComponents(     System.int RowIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RestoreRestructuredComponents(  &   System.int RowIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowIndex*
:   1-based row index, if more than one subassembly or weldment are dissolved; 0, if only one subassembly or weldment is dissolved

#### Return Value

True if the subassembly or weldment is restored, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomTableAnnotation::RestoreRestructuredComponents.

# ![](dotnetimages/collapse.gif)Example

[Dissolve Subassembly in a BOM Table (VBA)](Dissolve_Subassembly_in_a_BOM_Table_Example_VB.htm)

[Dissolve Subassembly in a BOM Table (VB.NET)](Dissolve_Subassembly_in_a_BOM_Table_Example_VBNET.htm)

[Dissolve Subassembly in a BOM Table (C#)](Dissolve_Subassembly_in_a_BOM_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::Dissolve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Dissolve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP5, Revision Number 20.5